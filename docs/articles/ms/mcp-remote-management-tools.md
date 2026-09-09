# Bagaimana memilih alat pengurusan jauh MCP? Perbandingan Bastrio dengan alat SSH, pangkalan data dan Docker

[Docs home / 文档首页](../../../README.md) · [Article index / 文章目录](README.md) · [All languages / 所有语言](../README.md)

Original / 原文: [https://bastr.io/ms/articles/mcp-remote-management-tools/](https://bastr.io/ms/articles/mcp-remote-management-tools/)

Languages / 语言: [English](../en/mcp-remote-management-tools.md) · [简体中文](../zh/mcp-remote-management-tools.md) · [繁體中文](../zh-TW/mcp-remote-management-tools.md) · [Español](../es/mcp-remote-management-tools.md) · [Deutsch](../de/mcp-remote-management-tools.md) · [Français](../fr/mcp-remote-management-tools.md) · [日本語](../ja/mcp-remote-management-tools.md) · [한국어](../ko/mcp-remote-management-tools.md) · [Bahasa Melayu](../ms/mcp-remote-management-tools.md) · [Русский](../ru/mcp-remote-management-tools.md)

> Menerangkan cara MCP menghubungkan AI dengan hos jauh melalui kebenaran, kelulusan manusia dan audit operasi, serta membandingkan Bastrio MCP, klien SSH, IDE pangkalan data, alat Docker dan desktop jauh RDP/VNC.

MCP (Model Context Protocol) membolehkan klien AI mengakses sumber jauh terkawal melalui alat piawai. Ia bukan menyerahkan kata laluan pelayan kepada AI; pelayan mendedahkan alat yang terhad skopnya, pengguna mengesahkan operasi berimpak tinggi, kemudian rekod boleh dikesan ditinggalkan.

Tarikh pengesahan maklumat: 11 Ogos 2026. Artikel ini membandingkan sempadan keupayaan dan aliran operasi; ia tidak menyifatkan "menyokong MCP" sebagai keselamatan automatik dan tidak menggunakan kedudukan prestasi tanpa syarat seragam.

## Kedudukan MCP dalam pengurusan jauh

Bastrio MCP menggunakan Streamable HTTP dan kunci API; senarai alat ditapis menurut scope yang dibenarkan. Klien AI boleh menemui alat, membaca maklumat hos dan ruang kerja, melihat fail atau menjalankan pertanyaan pangkalan data baca sahaja. Menulis fail, menjalankan arahan terminal, menulis pangkalan data, pemindahan fail dan operasi berimpak tinggi lain mengembalikan `approval_required` dan hanya dilaksanakan selepas pengguna mengesahkan dalam pelayar; sejarah operasi merekod permintaan serta hasil. Kata laluan, kekunci persendirian dan kelayakan dalaman tidak dikembalikan sebagai output alat; sumber dirujuk melalui pemegang legap.

![Ilustrasi pintu masuk SSH dalam talian Bastrio dan pengurusan jauh AI](../../images/articles/ssh-interface.png)

## Perbandingan keupayaan dengan alat biasa

- **Alat atau cara:** Bastrio MCP; **Pintu masuk utama:** klien AI + kelulusan pelayar; **Orkestrasi AI:** tugas merentas alat SSH, fail, pangkalan data dan Docker; **Kelulusan manusia dan audit:** pengesahan kedua serta jejak untuk operasi berimpak tinggi; **Senario lebih sesuai:** penyiasatan jauh, automasi terkawal, kerjasama pasukan
- **Alat atau cara:** MobaXterm / Xshell / SecureCRT; **Pintu masuk utama:** terminal desktop; **Orkestrasi AI:** bergantung pada skrip tempatan atau integrasi klien; **Kelulusan manusia dan audit:** bergantung pada proses pasukan; **Senario lebih sesuai:** terminal, sesi, skrip dan X11
- **Alat atau cara:** DBeaver / DataGrip / Navicat; **Pintu masuk utama:** IDE pangkalan data desktop; **Orkestrasi AI:** sesetengah produk mempunyai bantuan AI; **Kelulusan manusia dan audit:** bergantung pada tetapan pangkalan data dan klien; **Senario lebih sesuai:** pembangunan SQL, pemodelan dan analisis khusus
- **Alat atau cara:** Portainer / Dockge / Docker Desktop; **Pintu masuk utama:** antara muka Docker web atau desktop; **Orkestrasi AI:** mengikut integrasi produk; **Kelulusan manusia dan audit:** bergantung pada penggunaan dan konfigurasi akaun; **Senario lebih sesuai:** kontena, Compose dan pembangunan setempat
- **Alat atau cara:** Apache Guacamole / TeamViewer; **Pintu masuk utama:** antara muka RDP/VNC atau bantuan jauh; **Orkestrasi AI:** lazimnya bukan pintu masuk operasi MCP; **Kelulusan manusia dan audit:** bergantung pada keupayaan audit platform; **Senario lebih sesuai:** akses desktop grafik dan bantuan jauh

## Satu proses operasi AI yang selamat

1. Cipta kunci API MCP, berikan scope yang perlu sahaja dan serahkan kepada klien AI melalui pemboleh ubah persekitaran.
2. Minta klien menjalankan `tools/list`, sahkan alat yang benar-benar tersedia dan jangan membuat andaian berdasarkan bilangan alat tetap.
3. Minta dahulu bacaan keadaan, log atau pertanyaan baca sahaja; minta AI menerangkan sasaran, skop dan kesan yang dijangka.
4. Bagi operasi tulis, semak `approval_required`, ID operasi, masa tamat dan halaman kelulusan, kemudian sahkan atau batalkan dalam pelayar.
5. Selepas pelaksanaan, lihat sejarah operasi dan sahkan hos sasaran, laluan fail, syarat SQL atau nama kontena.

![Ilustrasi antara muka pengurusan Docker Bastrio dan senario orkestrasi MCP](../../images/articles/docker-scenarios.png)

## Rujukan

- [Panduan klien Bastrio MCP](https://bastr.io/ms/articles/mcp-ai-server-operations/)
- [Model Context Protocol](https://modelcontextprotocol.io/)
- [OpenSSH](https://www.openssh.com/)
- [Dokumentasi Docker](https://docs.docker.com/)
- [DBeaver](https://dbeaver.io/)
- [Portainer](https://www.portainer.io/)

Teruskan membaca: [Cadangan alat SSH](ssh-tools-browser-workspace.md); [Alat pengurusan visual Docker](docker-management-tools-by-scenario.md).

## FAQ

### Adakah MCP memberikan AI keistimewaan root pelayan secara automatik?

Tidak. Scope MCP, kebenaran ahli ruang kerja, kelayakan sambungan dan akaun hos sasaran bersama-sama mengehadkan apa yang boleh dilaksanakan.

### Mengapa membenarkan AI membaca keadaan sahaja, bukannya terus membaiki?

Diagnosis baca sahaja lebih mudah disemak dan tidak mengubah keadaan sistem. Operasi pembaikan boleh memberi kesan pada perkhidmatan, data atau kebenaran; periksa parameter dahulu, kemudian luluskan melalui pelayar.

### Bolehkah MCP menggantikan alat khusus SSH, pangkalan data atau Docker?

Ia lebih seperti lapisan orkestrasi terkawal dan pintu masuk AI, dan tidak perlu menggantikan semua klien khusus. SQL rumit, pembangunan Docker grafik, X11 atau desktop RDP/VNC lengkap masih mungkin memerlukan alat khusus.

### Apakah beza MCP Bastrio dengan WebSSH biasa?

WebSSH terutama menyediakan terminal pelayar; MCP membolehkan klien AI menemui dan memanggil banyak alat terkawal serta menghantar operasi berimpak tinggi ke aliran kelulusan manusia.

## Related articles / 相关文章

- [Cara menggunakan SSH dalam pelayar](https://bastr.io/ms/articles/online-ssh-in-browser/)
- [Cara membaiki SSH Permission denied (publickey)](https://bastr.io/ms/articles/ssh-permission-denied-publickey/)
- [Proksi Songsang WebSocket Nginx untuk WebSSH: Konfigurasi dan Seni Bina](https://bastr.io/ms/articles/nginx-websocket-webssh/)
