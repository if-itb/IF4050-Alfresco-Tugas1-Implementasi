Project ini merupakan contoh aplikasi yang menggunakan service pada Alfresco. Dikerjakan untuk memenuhi tugas eksplorasi Alfresco (community edition) dari matakuliah IF4050 Rekayasa Perangkat Lunak Berorientasi Service.

Anggota kelompok:

13509085 - Andre Novelando

13511026 - Akbar Juang Saputra

13512030 - Alvin Natawiguna

18211031 - Nicolas Novian Ruslim

13511078 - Taufik Hidayat

Cara Meng-install Alfresco (Windows)
1. Download file instalasi alfresco-enterprise-3.4.14-installer-win-x32.exe alfresco-enterprise-3.4.14-installer-win-x64.exe. Pilih file instalasi yang sesuai dengan versi OS.
2. Double-klik file untuk memulai proses instalasi.
3. Di jendela installation type, pilih cara yang dinginkan untuk menggunakan setup wizard.
   Ada 2 jenis tipe instalasi, yaitu Easy dan Advanced.
   - Easy : konfigurasi sudah diatur oleh setup wizard.
			hanya perlu memasukkan lokasi instalasi dan kata sandi administrator
   - Advanced : memperbolehkan mengatur server port dan service properties.
				dapat memilih komponen apa saja yang perlu diinstal
   
   Apabila memilih tipe Advanced maka harus mengikuti langkah selanjutnya.
   
4. Pilih komponen yang ingin diinstall.
5. Pilih lokasi folder instalasi.
6. Di jendela Database Server Parameters, masukkan port number untuk database yang digunakan.
7. Pada jendela Tomcat Port Configuration, masukkan parameter konfigurasi Tomcat sebagai berikut :
	a. Web server domain, contohnya secara default 127.0.0.1
	b. Tomcat port, contohnya secara default 8080
	c. Tomcat Shutdown port, contohnya secara default 8443
	d. Tomcat AJP port, contohnya secara default 8009
8. Pada jendela Alfresco FTP Port, masukkan angka port untuk Alfresco FTP server
9. Pada jendela Alfresco RMI Port, masukkan angka port untuk RMI service
10. Pada jendela Admin Password, masukkan password yang ingin digunakan
11. Pada jendela Service Startup Configuration, terdapat 2 pilihan mengatur service-nya
	- Manual : Atur agar service bekerja saat dijalankan manual.
	- Auto : Service akan langsung berjalan secara otomatis ketika alfresco dijalankan.
12. Klik Next pada jendela Ready to Install. Jendela Installing akan menunjukkan progress instalasi.
13. Instalasi selesai.
14. Buka (domain dari web server alfresco) http://127.0.0.1:8080/share
	(Proses membuka aplikasi akan memakan waktu beberapa menit)
15. Log on ke Alfresco Share sebagai admin.
16. Jalankan service apabila pada jendela Service Startup Configuration memilih Manual.
17. Untuk menghentikan Alfresco sepenuhnya, kita harus menghentikan semua service.
	Gunakan script di directory instalasi untuk memulai atau menghentikan service :
		servicerun start dan servicerun stop

Cara Penggunaan aplikasi:
1. Import project alfresco-cloud-example ke Eclipse atupun Netbeans.
2. Ubah nilai Alfresco_API_URL pada file BaseJavaExample.java menjadi domain yang telah kita buat sebelumnya.
3. Export project menjadi jar file.
4. Gunakan jar file yang telah dibuat menjadi library pada project Alfresco-mini-app.
5. Jalankan aplikasi Alfresco-mini-app.

SELAMAT MENCOBA
