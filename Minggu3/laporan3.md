# tekn-basis-data
# latihan
# Laporan-pertemuan-ke3

# Software yang Diperlukan

*Sistem Operasi: Linux, Windows, Mac, FreeBSD, dan sistem operasi lain yang mendukung MongoDB
*MongoDB Community Server. Pada saat download, pilih server di pilihan Package. Software yang didownload sudah termasuk mongo shell untuk mengakses MongoDB server. Pilihkan sesuai dengan sistem operasi yang anda gunakan pada pilihan OS.
*Python, bisa diperoleh via python.org atau Miniconda.
*Visual Studio Code dengan Python extension.

# Pembelanjaraan

1. Selain menggunakan mongosh (mongo Shell), data di MongoDB juga bisa dikelola menggunakan berbagai peranti pengembangan bahasa pemrograman. Berbagai bahasa pemrograman tersebut menggunakan driver untuk melakukan koneksi dan manipulasi data di MongoDB. Berbagai driver serta ODM dijelaskan pada dokumentasi driver - ODM untuk MongoDB.
2. Dokumentasi manual MongoDB bisa menjadi acuan jika ada hal-hal yang belum dipahami: databases dan collections, documents di MongoDB, perbandingan SQL dengan MongoDB, dan lain-lain.
3. Instalasi PyMongo, driver MongoDB untuk Python.
4. Tutorial penggunakan PyMongo.

# Latihan

pada latihan nomor 1 kita akan mengaktifkan MongoDB server setelah kita selesai mengaktifkannya kita akan beralih ke no 2 dengan menginstall python, cara menginstal seperti pada Buka file installer yang telah di download, kemudian pada  Centang Install launcher for all user untuk mengaktifkan python pada semua user Windows dan centang Python 3.6 to PATH untuk menambah path command Python. Kemudian klik Install Now. Klik Yes saat muncul notifikasi User Account Control.(Screenshot (1)
Selanjutnya Proses instal Python berjalan Screenshot (2) Tunggu proses install hingga selesai. kemudian Opsi “Disable path length limit”
Disini, anda dapat mengaktifkan atau menonaktifkan batasan lintasan direktori Python. Untuk pengguna Linux batasan ini tidak mempunyai pengaruh yang besar, karena Linux menyimpan python pada direktori yang pendek. Berbeda halnya dengan Windows, yang menyimpan direktori lintasan agak jauh dari direktori utama partisi. Disarankan untuk menonaktifkan batasan ini dengan klik “Disable path length limit“. selanjutnya instal Python berhasil kemudian klik Close untuk menutup Installer Pyton Screenshot (3).

Latihan no 3 Install Visual Studio Code serta extension untuk Python

Memulai dengan Python dalam Kode VS
Dalam tutorial ini, Anda menggunakan Python 3 untuk membuat aplikasi Python "Hello World" yang paling sederhana dalam Visual Studio Code. Dengan menggunakan ekstensi Python, Anda membuat VS Code menjadi Python IDE ringan yang hebat (yang dapat Anda temukan sebagai alternatif produktif untuk PyCharm).

Tutorial ini memperkenalkan Anda ke VS Code sebagai lingkungan Python, terutama cara mengedit, menjalankan, dan men-debug kode melalui tugas-tugas berikut:

Tulis, jalankan, dan debug Aplikasi Python "Hello World"
Pelajari cara menginstal paket dengan membuat lingkungan virtual Python
Tulis skrip Python sederhana untuk memplot angka dalam VS Code
Tutorial ini tidak dimaksudkan untuk mengajari Anda Python sendiri. Setelah Anda terbiasa dengan dasar-dasar Kode VS, Anda kemudian dapat mengikuti salah satu tutorial pemrograman di python.org dalam konteks Kode VS untuk pengantar bahasa.

Jika Anda memiliki masalah, jangan ragu untuk mengajukan masalah untuk tutorial ini di repositori dokumentasi VS Code.

Catatan: Anda dapat menggunakan VS Code dengan Python 2 dengan tutorial ini, tetapi Anda perlu membuat perubahan yang sesuai pada kode, yang tidak dibahas di sini.

Prasyarat
Untuk berhasil menyelesaikan tutorial ini, Anda harus terlebih dahulu mengatur lingkungan pengembangan Python Anda. Secara khusus, tutorial ini membutuhkan:

Kode VS
Ekstensi VS Code Python
Python 3
Instal Visual Studio Code dan Python Extension
Jika Anda belum melakukannya, instal VS Code

Selanjutnya, instal ekstensi Python untuk VS Code dari Visual Studio Marketplace. Untuk detail tambahan tentang menginstal ekstensi, lihat Extension Marketplace. Ekstensi Python bernama Python dan diterbitkan oleh Microsoft. seperti pada gambar Screenshot (6)

Windows
Instal Python dari python.org. Anda biasanya dapat menggunakan tombol Unduh Python yang muncul pertama kali di halaman untuk mengunduh versi terbaru.

Catatan: Jika Anda tidak memiliki akses admin, opsi tambahan untuk menginstal Python di Windows adalah menggunakan Microsoft Store. Microsoft Store menyediakan pemasangan Python 3.7 dan Python 3.8. Ketahuilah bahwa Anda mungkin memiliki masalah kompatibilitas dengan beberapa paket menggunakan metode ini.

Untuk informasi tambahan tentang Python di Windows, lihat Menggunakan Python pada Windows di Python.org

macOS
Instalasi sistem Python di macOS tidak didukung. Sebaliknya, instalasi melalui Homebrew disarankan. Untuk menginstal Python menggunakan Homebrew di macOS, gunakan brew install python3 di Terminal prompt.

Catatan Di macOS, pastikan lokasi pemasangan Kode VS Anda termasuk dalam variabel lingkungan PATH Anda. Lihat instruksi pengaturan ini untuk informasi lebih lanjut.

Linux
Instalasi Python 3 built-in di Linux berfungsi dengan baik, tetapi untuk menginstal paket Python lain Anda harus menginstal pip dengan get-pip.py.

Pilihan lain
Ilmu Data: Jika tujuan utama Anda menggunakan Python adalah Ilmu Data, maka Anda dapat mempertimbangkan untuk mengunduh dari Anaconda. Anaconda tidak hanya menyediakan juru bahasa Python, tetapi banyak perpustakaan dan alat yang berguna untuk ilmu data.

Subsistem Windows untuk Linux: Jika Anda bekerja pada Windows dan menginginkan lingkungan Linux untuk bekerja dengan Python, Windows Subsystem untuk Linux (WSL) adalah opsi untuk Anda. Jika Anda memilih opsi ini, Anda juga ingin menginstal ekstensi Remote - WSL. Untuk informasi lebih lanjut tentang menggunakan WSL dengan VS Code, lihat VS Code Remote Development atau coba tutorial Working in WSL, yang akan memandu Anda dalam mengatur WSL, menginstal Python, dan membuat aplikasi Hello World yang berjalan di WSL.

Verifikasi pemasangan Python
Untuk memverifikasi bahwa Anda telah berhasil menginstal Python di mesin Anda, jalankan salah satu dari perintah berikut (tergantung pada sistem operasi Anda):
seperti pada gambar Screenshot (7) dan Screenshot (8)

Buat file kode sumber Python Hello World
Dari toolbar File Explorer, pilih tombol File Baru pada folder halo:
 Beri nama file hello.py, dan secara otomatis terbuka di editor, Dengan menggunakan ekstensi file .py, Anda memberi tahu VS Code untuk menafsirkan file ini sebagai program Python, sehingga mengevaluasi konten dengan ekstensi Python dan juru bahasa yang dipilih.

Catatan: Toolbar File Explorer juga memungkinkan Anda membuat folder di dalam ruang kerja Anda untuk mengatur kode Anda dengan lebih baik. Anda dapat menggunakan tombol folder baru untuk membuat folder dengan cepat.

Sekarang Anda memiliki file kode di Workspace Anda, masukkan kode sumber berikut di hello.py:
 seperti pada gambar 
 ![Screenshot (9)](Screenshot (9).png) 
 dan Screenshot (10)

# kesimpulan 

 Mahasiswa dapat mengetahui Keterkaitan MongoDB dengan berbagai peranti pengembangan bahasa pemrograman.
dan Menggunakan driver Python untuk MongoDB (PyMongo) untuk mengakses Python