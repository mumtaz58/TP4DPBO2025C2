**Janji**

Saya Armelia Zahrah Mumtaz dengan NIM 2300801 berjanji mengerjakan TP4 DPBO dengan keberkahan-Nya, maka saya tidak akan melakukan kecurangan sesuai yang telah di spesifikasikan, Aamiin

**Desain Program**

Program ini adalah aplikasi manajemen data mahasiswa dengan GUI Java Swing. Berikut adalah class-class dalam desain program:

1. **Mahasiswa**: Class model yang menyimpan data mahasiswa
   - Atribut: nim, nama, jenisKelamin, jurusan
   - Method: constructor, getter, dan setter untuk semua atribut

2. **Menu**: Class utama yang membangun GUI dan implementasi logika program
   - Extends JFrame untuk membuat window aplikasi
   - Menggunakan ArrayList untuk menyimpan data mahasiswa
   - Menangani operasi CRUD (Create, Read, Update, Delete)
   - Berisi komponen GUI seperti JTextField, JTable, JButton, JComboBox, dll.

**Alur Program**

1. **Inisialisasi**:
   - Program dimulai dari method `main()` di class Menu
   - Membuat window dengan ukuran 480x600 pixel
   - Mengatur posisi window di tengah layar
   - Mengatur warna background menjadi biru pastel

2. **Setup Data dan Komponen**:
   - Inisialisasi ArrayList untuk menyimpan data mahasiswa
   - Mengisi data awal dengan method `populateList()`
   - Mengisi tabel mahasiswa dengan data dari ArrayList
   - Mengatur pilihan pada combo box untuk jenis kelamin dan jurusan
   - Mengatur font untuk judul

3. **Operasi CRUD**:
   - **Create (Insert)**:
     - User mengisi form (NIM, nama, jenis kelamin, jurusan)
     - Klik tombol "Add" untuk menambahkan data
     - Program memvalidasi input dan menambahkan mahasiswa baru ke ArrayList
     - Tabel diperbarui dan form dikosongkan

   - **Read**:
     - Data mahasiswa ditampilkan dalam tabel dengan kolom No, NIM, Nama, Jenis Kelamin, dan Jurusan
     - User dapat melihat semua data mahasiswa yang tersimpan

   - **Update**:
     - User mengklik baris pada tabel
     - Data dari baris yang dipilih ditampilkan pada form
     - Tombol "Add" berubah menjadi "Update" dan tombol "Delete" muncul
     - User mengubah data pada form dan mengklik "Update"
     - Data mahasiswa pada ArrayList diperbarui dan tabel direfresh

   - **Delete**:
     - User mengklik baris pada tabel
     - Tombol "Delete" muncul
     - User mengklik tombol "Delete"
     - Konfirmasi penghapusan ditampilkan
     - Jika konfirmasi "Ya", data dihapus dari ArrayList dan tabel direfresh

4. **Fungsi Tambahan**:
   - Tombol "Cancel" untuk membersihkan form dan reset status
   - Validasi input untuk memastikan semua field diisi
   - Feedback berupa pesan pop-up setelah operasi CRUD berhasil dilakukan
   - Tampilan visual yang menarik dengan warna biru pastel

Alur ini membentuk sistem CRUD sederhana untuk manajemen data mahasiswa dengan interface yang user-friendly dan validasi dasar untuk memastikan integritas data.
