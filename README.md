<div align="center">

# <span style="color:#60A5FA;">Flat</span><span style="color:#10284F;">Smart</span>
### *Sistem Informasi Operasional Minimarket & Decision Support System*

[![Java](https://img.shields.io/badge/Java-17%20LTS-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)](https://www.oracle.com/java/)
[![Swing](https://img.shields.io/badge/GUI-Java%20Swing-5382a1?style=for-the-badge&logo=java&logoColor=white)](https://docs.oracle.com/javase/8/docs/technotes/guides/swing/)
[![NetBeans](https://img.shields.io/badge/IDE-Apache%20NetBeans-1B6AC6?style=for-the-badge&logo=apache&logoColor=white)](https://netbeans.apache.org/)
[![MySQL](https://img.shields.io/badge/Database-MySQL%208.x-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Figma](https://img.shields.io/badge/Design-Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://www.figma.com/)
[![GitHub](https://img.shields.io/badge/VCS-GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)
[![Maven](https://img.shields.io/badge/Build-Apache%20Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)](https://maven.apache.org/)

<br/>

**Aplikasi desktop operasional minimarket berbasis Java Swing & MySQL yang mengolah data transaksi kasir menjadi tren penjualan harian, rekomendasi promosi batch (FIFO), dan analisis efektivitas omzet untuk mendukung keputusan manajer secara presisi.**

<br/>

[🏷️ Nama Program](#️-nama-program) •
[📝 Deskripsi Singkat](#-deskripsi-singkat) •
[🧩 Fitur Utama](#-fitur-utama-program) •
[🧱 Tech Stack](#-tech-stack-bahasa-database-framework-library) •
[📐 Perancangan Sistem](#-perancangan-sistem-flowchart-use-case-erd) •
[📁 Struktur Package](#-struktur-folder--package) •
[🎯 4 Pilar OOP](#-penjelasan-penerapan-4-pilar-oop-di-dalam-program) •
[▶️ Cara Penggunaan](#️-cara-penggunaan-program-sertakan-screenshot-gui) •
[👥 Kontributor](#-kontributor-nama-dan-nim)

---

### 🖥️ Antarmuka Ruang Kerja Sistem

| 🧑‍💼 Ruang Kerja Kasir (Point of Sale) | 👨‍💼 Ruang Kerja Manajer (Decision Support) |
|:---:|:---:|
| <img src="docs/gambar/fitur/Home%20Kasir.png" alt="Ruang Kasir" width="480"/> | <img src="docs/gambar/fitur/Home%20Manajer.png" alt="Ruang Manajer" width="480"/> |
| *Pencarian cepat barcode, Smart FIFO, auto-promo, & struk thermal* | *Kartu KPI, grafik tren omzet, prioritas batch expired, & export Excel* |

</div>

---

<a id="️-nama-program"></a>
## 🏷️ Nama Program

<div align="center">
  <br/>
  <h1 style="font-size: 64px; font-weight: 900; letter-spacing: -1px; margin: 0; line-height: 1.1;">
    <span style="color: #60A5FA;">Flat</span><span style="color: #10284F;">Smart</span>
  </h1>
  <p style="font-size: 19px; font-weight: 700; color: #1E3A8A; margin-top: 8px; margin-bottom: 6px; letter-spacing: 0.5px;">
    SISTEM INFORMASI OPERASIONAL MINIMARKET & DECISION SUPPORT SYSTEM
  </p>
  <p style="font-size: 14px; color: #475569; max-width: 720px; margin: 0 auto 16px auto;">
    Aplikasi Desktop Berbasis <b>Java 17 LTS</b> • <b>Java Swing</b> • <b>MySQL</b> • <b>Apache NetBeans</b> • <b>Figma</b> • <b>GitHub</b><br/>
    <i>Program Studi Sistem Informasi • Fakultas Teknik • Universitas Mulawarman (2026)</i>
  </p>
  <div style="display: flex; gap: 8px; justify-content: center; flex-wrap: wrap;">
    <span style="background: #10284F; color: #FFFFFF; padding: 5px 14px; border-radius: 20px; font-size: 12px; font-weight: 600;">v1.0 Capstone Release</span>
    <span style="background: #60A5FA; color: #0F172A; padding: 5px 14px; border-radius: 20px; font-size: 12px; font-weight: 700;">5-Layer MVC + DAO</span>
    <span style="background: #E2E8F0; color: #1E293B; padding: 5px 14px; border-radius: 20px; font-size: 12px; font-weight: 600;">Custom Connection Pooling</span>
    <span style="background: #10B981; color: #FFFFFF; padding: 5px 14px; border-radius: 20px; font-size: 12px; font-weight: 600;">Offline-First Desktop</span>
  </div>
  <br/>
</div>

---

<a id="-deskripsi-singkat"></a>
## 📝 Deskripsi Singkat

### 💡 Latar Belakang Masalah
Pada operasional minimarket konvensional, transaksi penjualan harian umumnya hanya berhenti sebagai arsip kertas struk atau baris data mentah yang tidak diolah. Akibatnya:
1. **Manajer kesulitan memantau tren**: Tidak diketahui pasti produk mana yang paling mendongkrak omzet vs produk yang mengalami perlambatan (*dead stock*).
2. **Promosi tidak efektif**: Program diskon kerap dipasang acak tanpa melihat usia simpan (*shelf life*) produk.
3. **Kerugian barang kedaluwarsa**: Produk lama tertimbun di rak belakang hingga melewati masa kedaluwarsa karena tidak menerapkan pengeluaran berbasis FIFO (*First In, First Out*).

### ✨ Solusi yang Dihadirkan FlatSmart
**FlatSmart** mentransformasikan seluruh transaksi kasir menjadi **dasbor visual tren penjualan**, **penilaian efektivitas promosi**, serta **rekomendasi cerdas pemotongan diskon batch**. Sistem ini menghubungkan aktivitas operasional kasir di meja depan (*Front Office*) dengan pengambilan keputusan manajerial (*Back Office*) secara terintegrasi.

```
❌ Masalah Minimarket Konvensional           ✨ Solusi Cerdas FlatSmart
┌──────────────────────────────────────┐     ┌──────────────────────────────────────┐
│ • Transaksi menumpuk tanpa analisis │     │ • Visualisasi Tren Omzet Harian      │
│ • Barang expired lolos pengawasan    │ ──▶ │ • Smart FIFO Batch & Auto-Promo      │
│ • Diskon acak & tidak terukur        │     │ • Evaluasi Efektivitas Promo         │
│ • Potensi data korup manual          │     │ • Transaksi SQL Atomik (Commit/Roll) │
└──────────────────────────────────────┘     └──────────────────────────────────────┘
```

### 🌟 6 Manfaat Utama
1. **Keputusan Berbasis Data Riil**: Manajer dapat membaca grafik tren omzet harian dan matriks kinerja produk (`Terlaris`, `Normal`, `Lambat`) tanpa mengira-ngira.
2. **Promosi Tepat Sasaran**: Sistem otomatis menyarankan produk lambat laku dan mendekati masa kedaluwarsa untuk segera diberi diskon cuci gudang.
3. **Efektivitas Promosi Terukur**: Membandingkan langsung nilai omzet, unit terjual, dan total potongan promosi untuk menentukan diskon mana yang menguntungkan.
4. **Meningkatkan Peluang Omzet**: Ketersediaan produk terlaris selalu terpantau lewat indikator stok menipis, mencegah hilangnya potensi transaksi.
5. **Mitigasi Kerugian Produk Expired**: Algoritma Smart FIFO memastikan barang dengan kedaluwarsa terdekat otomatis terpilih di kasir.
6. **Integritas Transaksi Tinggi**: Header transaksi, detail item belanja, dan pengurangan stok dieksekusi dalam **satu transaksi SQL atomik** (Anti-gagal sebagian).

### 🎯 Keterkaitan Sustainable Development Goals (SDGs)
Proyek perancangan FlatSmart mengacu pada 3 pilar SDGs:
* **SDGs 8 (Decent Work and Economic Growth)**: Mendorong pertumbuhan ekonomi inklusif dan efisiensi operasional minimarket melalui pengolahan data penjualan riil untuk penentuan strategi omzet dan efisiensi kerja staf.
* **SDGs 9 (Industry, Innovation, and Infrastructure)**: Membangun infrastruktur digital dan standardisasi sistem informasi minimarket yang terintegrasi, andal, dan siap mendukung inovasi ritel.
* **SDGs 12 (Responsible Consumption and Production)**: Meminimalkan limbah barang terbuang (*product waste*) melalui deteksi dini produk lambat laku dan mendekati kedaluwarsa via algoritma Smart FIFO dan promosi dini.

---

<a id="-fitur-utama-program"></a>
## 🧩 Fitur Utama Program

Aplikasi memisahkan hak akses secara ketat (*Role-Based Access Control*) berdasarkan akun login di database:

```
                            ┌────────────────────────┐
                            │  🔐 Login Multi-Role   │
                            └───────────┬────────────┘
                                        │
                 ┌──────────────────────┴──────────────────────┐
                 ▼                                             ▼
     ┌───────────────────────┐                     ┌───────────────────────┐
     │   🧑‍💼 RUANG KASIR      │                     │   👨‍💼 RUANG MANAJER    │
     ├───────────────────────┤                     ├───────────────────────┤
     │ 1. Transaksi Penjualan│                     │ 1. CRUD Produk & Batch│
     │ 2. Saran Barcode Auto │                     │ 2. CRUD Diskon Promo  │
     │ 3. Smart FIFO Promo   │                     │ 3. Monitoring Expired │
     │ 4. Cetak Struk 40-Col │                     │ 4. Dasbor KPI & Tren  │
     │ 5. Bayar Tagihan PPOB │                     │ 5. Analisis Produk    │
     │ 6. Riwayat Transaksi  │                     │ 6. Jembatan Promo     │
     │                       │                     │ 7. Ekspor Excel .xlsx │
     └───────────────────────┘                     └───────────────────────┘
```

<br/>

### 🛒 A. Fitur Ruang Kasir (Point of Sale)

<details open>
<summary><b>🔍 Rincian Fitur Ruang Kerja Kasir</b></summary>
<br/>

#### 1. Autentikasi & Pemisahan Role Login
Memverifikasi username dan password pengguna ke tabel `pengguna`. Sesi login tersimpan di `util/Sesi` dan sistem otomatis mengarahkan ke `KasirFrame` atau `ManajerFrame`.
* *File Kode*: `view/LoginFrame.java`, `controller/AuthController.java`, `dao/PenggunaDAO.java`

<p align="center">
  <img src="docs/gambar/penggunaan/Home%20Kasir.png" alt="Layar Kasir" width="750"/>
  <br/><em>Ruang kerja kasir siap transaksi setelah berhasil login</em>
</p>

#### 2. Transaksi Cepat & Keranjang Belanja Otomatis
Kasir dapat mengetik sebagian barcode atau nama produk. Sistem otomatis mencari produk yang stoknya masih tersedia tanpa perlu menghafal kode barcode.
* *File Kode*: `view/TransaksiPenjualan.java`, `PenjualanController.saranProduk()`

<p align="center">
  <img src="docs/gambar/penggunaan/Kasir%20Keranjang.png" alt="Keranjang Belanja" width="750"/>
  <br/><em>Daftar item belanjaan masuk ke tabel keranjang beserta kalkulasi harga</em>
</p>

#### 3. Smart FIFO Batch & Potongan Diskon Otomatis
Setiap barang yang ditambahkan ke keranjang otomatis mengambil batch stok dengan **tanggal kedaluwarsa terdekat** yang masih valid. Jika batch tersebut memiliki promo aktif, sistem langsung memotong harga secara otomatis.
* *File Kode*: `service/PenjualanService.java`, `dao/StokDAO.cariBatchTerkeluar()`

#### 4. Pembayaran, Kembalian, & Konfirmasi Sukses Transaksi
Mendukung pembayaran Tunai, QRIS, dan Kartu Debit. Mengkalkulasi subtotal, potongan diskon, total akhir, uang diterima, dan kembalian secara otomatis. Seluruh proses disimpan dalam **1 Transaksi SQL Atomik** (header + detail + pengurangan stok).
* *File Kode*: `view/TransaksiPenjualan.java`, `PenjualanController.proses()`

<p align="center">
  <img src="docs/gambar/penggunaan/Pembayaran.png" alt="Dialog Pembayaran" width="450"/>
  <br/><em>Dialog input pembayaran dan kalkulasi kembalian otomatis</em>
</p>

#### 5. Cetak Struk 40-Kolom (Thermal Printer Ready)
Menyajikan pratinjau struk berformat monospaced 40 karakter yang kompatibel langsung dengan printer thermal kasir 58mm.
* *File Kode*: `view/StrukDialog.java`, `service/RiwayatService.generateStruk()`

<p align="center">
  <img src="docs/gambar/penggunaan/Struk.png" alt="Pratinjau Struk" width="450"/>
  <br/><em>Pratinjau format cetak struk thermal 40-kolom</em>
</p>

#### 6. Pembayaran Tagihan / PPOB (Pulsa, PLN, PDAM)
Mencatat transaksi pembayaran tagihan eksternal, validasi format ID pelanggan, dan menambahkan biaya admin otomatis (Rp2.500) ke dalam transaksi.
* *File Kode*: `view/PembayaranTagihan.java`, `controller/TagihanController.java`

<p align="center">
  <img src="docs/gambar/penggunaan/Pembayaran%20tagihan.png" alt="Pembayaran Tagihan" width="750"/>
  <br/><em>Form pembayaran tagihan pelanggan dengan biaya admin otomatis</em>
</p>

#### 7. Riwayat Transaksi & Cetak Ulang Struk
Memungkinkan kasir meninjau kembali transaksi, memfilter rentang tanggal atau kata kunci, serta mencetak ulang struk lama jika diminta pembeli.
* *File Kode*: `view/LihatTransaksi.java`, `controller/TransaksiController.java`

<p align="center">
  <img src="docs/gambar/penggunaan/Lihat%20transaksi.png" alt="Riwayat Transaksi" width="750"/>
  <br/><em>Daftar riwayat transaksi kasir dengan filter pencarian dan opsi buka struk</em>
</p>

</details>

<br/>

### 📊 B. Fitur Ruang Manajer (Decision Support System)

<details open>
<summary><b>🔍 Rincian Fitur Ruang Kerja Manajer</b></summary>
<br/>

#### 8. CRUD Produk & Manajemen Batch Stok
Manajer dapat menambah, mengedit, dan mencari produk. Penambahan produk baru otomatis membuat **batch stok perdana** beserta tanggal kedaluwarsanya. Dilengkapi proteksi: produk yang pernah ditransaksikan tidak dapat dihapus (*Foreign Key Integrity*).
* *File Kode*: `view/KelolaProduk.java`, `controller/ProdukController.java`, `dao/ProdukDAO.java`

<p align="center">
  <img src="docs/gambar/penggunaan/Home%20Manajer.png" alt="Kelola Produk" width="750"/>
  <br/><em>Dasbor utama manajer: kelola master produk dan pemantauan stok menipis</em>
</p>

<p align="center">
  <img src="docs/gambar/penggunaan/Tambah%20produk.png" alt="Tambah Produk" width="450"/>
  <br/><em>Form penambahan produk baru beserta batch stok awal dan tanggal expired</em>
</p>

#### 9. CRUD Promosi Bertarget Batch
Manajer dapat membuat kode promosi (misal: `prm-001`), diskon 1% - 100%, dan mengaitkannya ke batch stok spesifik. Status promosi (`Akan datang`, `Aktif`, `Berakhir`) dihitung dinamis dari tanggal sistem.
* *File Kode*: `view/KelolaPromosi.java`, `controller/PromosiController.java`, `dao/PromosiDAO.java`

<p align="center">
  <img src="docs/gambar/penggunaan/Tambah%20Promosi.png" alt="Tambah Promosi" width="450"/>
  <br/><em>Form pembuatan promosi diskon yang ditargetkan pada batch produk tertentu</em>
</p>

#### 10. Pemantauan Stok Menipis & Batch Kedaluwarsa
Mengklik baris produk akan membuka rincian nomor batch, kuantitas unit, dan tanggal kedaluwarsa di bawah tabel.
* *File Kode*: `view/KelolaProduk.java`, `dao/StokDAO.cariBatch()`

<p align="center">
  <img src="docs/gambar/penggunaan/Batch%20produk.png" alt="Rincian Batch" width="650"/>
  <br/><em>Panel inspeksi batch stok produk terpilih</em>
</p>

#### 11. Dasbor Analisis KPI & Grafik Tren Omzet Harian
Menampilkan ringkasan total omzet, unit terjual, jumlah transaksi, dan diskon. Dilengkapi **Grafik Batang Tren Omzet Harian** yang digambar langsung di panel Swing (`Graphics2D`) dengan garis rata-rata omzet.
* *File Kode*: `view/AnalisisPenjualan.java`, `controller/AnalisisController.java`

<p align="center">
  <img src="docs/gambar/penggunaan/Analisis%20penjualan.png" alt="Analisis Penjualan" width="750"/>
  <br/><em>Dasbor visual omzet: kartu metrik KPI dan grafik batang tren harian</em>
</p>

#### 12. Rekomendasi Cepat: Jembatan Prioritas ke Promosi
Kartu *Prioritas Persediaan* mendeteksi batch yang mendekati expired. Klik tombol **Tinjau diskon batch di Kelola Promosi** untuk langsung berpindah ke menu promo dengan ID batch yang telah terpilih otomatis.

<p align="center">
  <img src="docs/gambar/penggunaan/Tinjauan%20diskon.png" alt="Tinjauan Diskon" width="450"/>
  <br/><em>Kartu rekomendasi penanganan batch yang mendekati masa kedaluwarsa</em>
</p>

#### 13. Drill-Down Riwayat Detail Transaksi Produk
Klik-ganda pada baris produk di tabel analisis untuk membuka riwayat transaksi lengkap barang tersebut selama rentang periode yang sedang dianalisis.
* *File Kode*: `view/DetailPenjualanProdukDialog.java`

<p align="center">
  <img src="docs/gambar/penggunaan/Detail%20produk.png" alt="Detail Transaksi Produk" width="750"/>
  <br/><em>Dialog riwayat detail penjualan per transaksi untuk produk terpilih</em>
</p>

#### 14. Ekspor Laporan Analisis ke Excel (.xlsx) 4-Sheet
Menyimpan rekapitulasi data analisis ke berkas Excel resmi (`.xlsx`) yang terbagi dalam 4 Sheet: *Ringkasan*, *Rincian Produk*, *Tren Harian*, dan *Detail Transaksi*.
> 🚀 **Inovasi Teknis**: Generator Excel dibangun murni (`util/ExcelWriter.java`) menggunakan standar Open Packaging Conventions via `java.util.zip` tanpa memerlukan library eksternal berukuran besar seperti Apache POI!

<p align="center">
  <img src="docs/gambar/penggunaan/Export%20excel.png" alt="Export Excel" width="600"/>
  <br/><em>Notifikasi konfirmasi laporan berhasil diekspor ke berkas Excel resmi</em>
</p>

</details>

---

<a id="-tech-stack-bahasa-database-framework-library"></a>
## 🧱 Tech Stack (Bahasa, Database, Framework, Library)

Sistem FlatSmart dibangun menggunakan tumpukan teknologi modern, efisien, dan andal yang dikelompokkan sesuai ketentuan proyek:

<div align="center">

```
┌────────────────────────────────────────────────────────────────────────┐
│                     DESAIN, IDE & VERSION CONTROL                      │
│        🎨 Figma (UI/UX)  •  💻 Apache NetBeans  •  🐙 GitHub (VCS)     │
└───────────────────────────────────┬────────────────────────────────────┘
                                    │
┌───────────────────────────────────▼────────────────────────────────────┐
│                       BAHASA & GUI FRAMEWORK                           │
│          ☕ Java 17 LTS   •   🖼️ Java Swing (NetBeans Matisse)          │
└───────────────────────────────────┬────────────────────────────────────┘
                                    │
┌───────────────────────────────────▼────────────────────────────────────┐
│                    DATABASE, POOLING & DRIVERS                         │
│  🗄️ MySQL / Laragon / XAMPP  •  🔌 Connector/J 9.4.0  •  🏊 Pool (5)   │
└───────────────────────────────────┬────────────────────────────────────┘
                                    │
┌───────────────────────────────────▼────────────────────────────────────┐
│                     CUSTOM LIBRARIES & ENGINES                         │
│  📊 Native Graphics2D Chart • 📑 OOXML ExcelWriter • 📅 DatePicker Util│
└────────────────────────────────────────────────────────────────────────┘
```

</div>

<br/>

| Kategori | Teknologi | Versi | Peran dalam FlatSmart | Alasan Pemilihan Teknis |
|---|---|:---:|---|---|
| **Bahasa Pemrograman** | **Java** | 17 LTS | Bahasa utama seluruh lapisan sistem (Model, View, Controller, Service, DAO, Utility). | Mendukung 4 pilar OOP murni, *strict type safety*, performa eksekusi tinggi, dan kompatibilitas jangka panjang. |
| **Integrated Dev Environment** | **Apache NetBeans** | 18+ / 21+ | Lingkungan pengembangan utama (IDE), manajemen proyek Maven, runner `nbactions.xml`, dan debugging visual. | IDE standar resmi kurikulum PBO dengan dukungan native GUI Builder Matisse untuk mendesain berkas `.form` Swing secara visual. |
| **Database** | **MySQL / MariaDB** | 8.x / 10.4 (Laragon / XAMPP) | Basis data relasional `db_flatsmart` (8 tabel ACID, Foreign Key, Cascade). | Standar industri yang andal untuk transaksi ACID (*Atomicity, Consistency, Isolation, Durability*) dan mudah dikelola lewat Laragon / XAMPP. |
| **GUI Framework** | **Java Swing (JFC)** | Bawaan JDK | Kerangka antarmuka pengguna desktop: `JFrame`, `JDialog`, `JTable`, `JTextArea`. | Standar desktop kurikulum PBO, tidak memerlukan instalasi dependensi runtime tambahan, dan responsif. |
| **GUI Builder** | **NetBeans Matisse** | Bawaan NetBeans | Perancang antarmuka visual dua arah (menghasilkan berkas `.form` dan blok Java yang sinkron). | Mempermudah penataan tata letak visual komponen secara cepat, presisi, dan terintegrasi langsung di NetBeans. |
| **Layout Manager** | **AbsoluteLayout** | Snapshot | Pengatur posisi pixel-perfect pada form kartu, breadcrumb, dan dasbor. | Menjaga konsistensi posisi komponen UI agar tidak bergeser saat ukuran panel berubah. |
| **Database Driver** | **MySQL Connector/J** | 9.4.0 | Jembatan komunikasi JDBC antara aplikasi Java dan MySQL server via `DriverManager`. | Driver JDBC resmi dari Oracle/MySQL dengan dukungan protokol koneksi terbaru. |
| **Desain Antarmuka** | **Figma** | Cloud | Perancangan prototipe UI/UX, penentuan *color palette*, hirarki visual, dan tipografi. | Memastikan antarmuka kasir dan dasbor manajer memiliki pengalaman pengguna (UX) yang intuitif sebelum dikodekan. |
| **Version Control** | **GitHub / Git** | 2.x | Pelacakan riwayat kode, kolaborasi antar anggota tim, issue tracking, dan backup kode. | Memudahkan kolaborasi pengembangan tim, kontrol versi berkas, dan dokumentasi repositori proyek. |
| **Build Tool** | **Apache Maven** | 4.0.0 | Manajemen dependensi tunggal (`pom.xml`), kompilasi kode, dan runner konfigurasi. | Standar otomatisasi build Java modern; memastikan dependensi terunduh seragam di setiap komputer tim. |
| **Reporting Engine** | **`ExcelWriter` (Custom)** | Internal | Library generator berkas `.xlsx` 4-sheet berbasis OOXML murni memakai `java.util.zip`. | Menghasilkan berkas Excel resmi tanpa membebani ukuran aplikasi dengan library besar seperti Apache POI. |
| **Connection Pooling**| **Custom Pool Engine** | Internal | Mengelola kolam daur ulang 5 koneksi fisik database (`DatabaseConnection.java`). | Mengeliminasi latensi *handshake* koneksi berulang pada kueri intensif kasir. |

---

<a id="-perancangan-sistem-flowchart-use-case-erd"></a>
## 📐 Perancangan Sistem (Flowchart, Use Case, ERD)

Perancangan sistem FlatSmart mengacu langsung pada dokumen resmi **Laporan Project Akhir Praktikum Sistem Basis Data — Program Studi Sistem Informasi Universitas Mulawarman**.

---

### 1. 📊 Flowchart Sistem (Alur Kerja Operasional)

<details open>
<summary><b>🔍 Rincian 5 Flowchart Sistem</b></summary>
<br/>

#### A. Flowchart Menu Login
Menggambarkan proses autentikasi pengguna saat mengakses FlatSmart. Dimulai dengan memeriksa input username dan password. Jika tidak valid, sistem menampilkan pesan data tidak ditemukan. Jika valid, sistem memeriksa role: akun manajer melakukan sinkronisasi database manajer dan menampilkan `ManajerFrame`, sedangkan akun kasir melakukan sinkronisasi database kasir dan menampilkan `KasirFrame`.

```mermaid
flowchart TD
  A([Mulai]) --> B[Tampilkan Menu Login]
  B --> C{Apakah Login?}
  C -->|Tidak| Z([Selesai])
  C -->|Ya| D[Input Username & Password]
  D --> E{Apakah Data Valid?}
  E -->|Tidak| F[Data Tidak Ditemukan] --> B
  E -->|Ya| G{Apakah Akun Kasir?}
  G -->|Ya| H[Sinkronisasi Database Akun Kasir] --> I[Tampilkan Menu Kasir] --> J([Menu Kasir])
  G -->|Tidak| K{Apakah Akun Manajer?}
  K -->|Ya| L[Sinkronisasi Database Akun Manajer] --> M[Tampilkan Menu Manajer] --> N([Menu Manajer])
```

<p align="center">
  <img src="docs/gambar/perancangan/FlatSmart-Menu%20login.drawio.png" alt="Flowchart Menu Login" width="700"/>
  <br/><em>Alur autentikasi dan validasi role akun pengguna</em>
</p>

---

#### B. Flowchart Menu Kasir
Kasir dapat memilih fitur: **Pembayaran Produk**, **Pembayaran Tagihan**, **Riwayat Transaksi**, atau **Keluar**.
- Pada pembayaran produk: kasir memasukkan barcode produk, sistem memvalidasi stok, kasir menginput kuantitas, sistem menghitung total beserta promo aktif, kasir memilih metode bayar, menginput uang diterima, menghitung kembalian, menampilkan struk, dan menyimpan riwayat transaksi.
- Pada pembayaran tagihan: kasir memilih jenis tagihan, sistem memvalidasi, kasir menginput nomor pelanggan, nama, dan nominal, sistem menghitung total ditambah biaya admin (Rp2.500), menampilkan struk, dan menyimpan riwayat transaksi.

```mermaid
flowchart TD
  A([Mulai Menu Kasir]) --> B{Pilih Menu Kasir}
  B -->|Pembayaran Produk| C[Tampilkan Transaksi Penjualan]
  C --> D[Input / Scan Barcode Produk]
  D --> E{Validasi Produk & Stok?}
  E -->|Tidak Cukup| F[Peringatan Stok] --> D
  E -->|Valid| G[Input Jumlah Barang]
  G --> H[Hitung Total Pembayaran & Promo Aktif]
  H --> I[Pilih Metode Pembayaran & Input Uang]
  I --> J{Uang Cukup?}
  J -->|Kurang| I
  J -->|Ya| K[Hitung Kembalian, Cetak Struk, Simpan Transaksi]
  
  B -->|Pembayaran Tagihan| L[Pilih Jenis Tagihan: Listrik/Air/Pulsa/BPJS]
  L --> M[Input Nomor Pelanggan, Nama & Nominal]
  M --> N[Hitung Total Tagihan + Biaya Admin Rp2.500]
  N --> O[Proses Bayar, Cetak Bukti, Simpan Riwayat]
  
  B -->|Riwayat Transaksi| P[Tampilkan Riwayat Transaksi & Filter]
  B -->|Keluar| Q[Kembali ke Menu Login]
```

<p align="center">
  <img src="docs/gambar/perancangan/FlatSmart-Menu%20Kasir.drawio.png" alt="Flowchart Menu Kasir" width="700"/>
  <br/><em>Alur operasional ruang kerja kasir (POS dan pembayaran tagihan)</em>
</p>

---

#### C. Flowchart Menu Manajer
Menggambarkan 4 pilihan menu utama manajer: **Kelola Produk**, **Kelola Promosi**, **Analisis Penjualan**, dan **Keluar**. Pada analisis penjualan, manajer menentukan tanggal awal dan tanggal akhir. Sistem memvalidasi tanggal (tanggal akhir tidak boleh lebih awal dari tanggal awal), menghitung total omzet, jumlah produk terjual, klasifikasi produk (`Terlaris`, `Normal`, `Lambat`), dan menampilkan rincian hasil analisis.

```mermaid
flowchart TD
  A([Mulai Menu Manajer]) --> B{Pilih Menu Manajer}
  B -->|Kelola Produk| C([Arahkan ke Menu Kelola Produk])
  B -->|Kelola Promosi| D([Arahkan ke Menu Kelola Promosi])
  B -->|Analisis Penjualan| E[Input Tanggal Awal & Tanggal Akhir]
  E --> F{Validasi Format & Rentang Tanggal?}
  F -->|Tidak Valid| G[Peringatan Tanggal Salah] --> E
  F -->|Valid| H[Hitung Total Omzet & Jumlah Terjual]
  H --> I[Klasifikasikan Produk: Terlaris / Normal / Lambat]
  I --> J[Tampilkan Rincian Hasil Analisis Penjualan]
  B -->|Keluar| K[Konfirmasi Keluar ➡️ Kembali ke Login]
```

<p align="center">
  <img src="docs/gambar/perancangan/FlatSmart-Menu%20Manajer.drawio.png" alt="Flowchart Menu Manajer" width="700"/>
  <br/><em>Alur navigasi dan analisis penjualan manajer</em>
</p>

---

#### D. Flowchart Menu Kelola Produk
Menyediakan lima pilihan: **Menampilkan**, **Menambah**, **Memperbarui**, **Menghapus Produk**, dan **Keluar**.
- Tambah: menginput barcode, nama, harga beli, harga jual, stok, dan tanggal kedaluwarsa batch pertama.
- Perbarui: validasi barcode, menampilkan detail, menginput harga baru, dan menyimpan pembaruan.
- Hapus: validasi barcode, menampilkan detail, meminta konfirmasi, dan menghapus dari database (ditolak jika pernah ditransaksikan).

<p align="center">
  <img src="docs/gambar/perancangan/FlatSmart-Menu%20kelola%20produk.drawio.png" alt="Flowchart Kelola Produk" width="700"/>
  <br/><em>Alur pengelolaan master produk dan inventaris batch</em>
</p>

---

#### E. Flowchart Menu Kelola Promosi
Menyediakan pilihan: **Menampilkan**, **Menambah**, **Menghapus Promosi**, dan **Keluar**.
- Tambah: memasukkan nama promosi dan barcode produk, sistem memvalidasi produk, manajer memasukkan persentase diskon serta tanggal mulai dan tanggal selesai promosi. Sistem mengenerate kode promosi otomatis (`prm-xxx`) dan menyimpannya ke database.
- Hapus: sistem menampilkan daftar promosi, meminta kode promosi yang akan dihapus, validasi, meminta konfirmasi, dan menghapus dari database.

<p align="center">
  <img src="docs/gambar/perancangan/FlatSmart-Menu%20Kelola%20Promosi.drawio.png" alt="Flowchart Kelola Promosi" width="700"/>
  <br/><em>Alur perancangan dan penghapusan promosi diskon</em>
</p>

</details>

---

### 2. 👤 Use Case Diagram (Alur Use Case Sistem)

<details open>
<summary><b>🔍 Rincian Use Case Diagram</b></summary>
<br/>

Sesuai dengan rancangan sistem FlatSmart, sistem memetakan interaksi dua aktor utama (**Kasir** dan **Manajer**):
* **Kasir**: Melakukan login, mengelola keranjang belanja (`<<extend>>` Tambah, Ubah, Hapus), melakukan pembayaran produk dengan kalkulasi total bayar (`<<include>>` Memproses Pembayaran yang mencakup pemilihan metode bayar, kalkulasi kembalian, dan simpan riwayat), menampilkan struk (`<<include>>` Cetak Struk), melakukan pembayaran tagihan (PPOB), dan melihat riwayat transaksi.
* **Manajer**: Melakukan login, mengelola produk (`<<extend>>` Tambah, Update, Hapus), mengelola promosi (`<<extend>>` Tambah, Hapus), serta melihat analisis penjualan (`<<include>>` Melihat Rincian Produk, Melihat Total Omset, Melihat Jumlah Produk Terjual, dan Mengklasifikasikan Produk).

```mermaid
flowchart LR
  kasir([🧑‍💼 Kasir])
  manajer([👨‍💼 Manajer])

  subgraph FlatSmart ["Sistem Informasi Operasional FlatSmart"]
    login(("🔐 Login"))

    subgraph KasirScope ["Ruang Kasir (Point of Sale)"]
      bayarProduk(("Pembayaran Produk"))
      bayarTagihan(("Pembayaran Tagihan"))
      riwayatTrx(("Melihat Riwayat Transaksi"))
      
      kelolaKeranjang(("Kelola Keranjang"))
      tambahItemKeranjang(("Tambah Produk"))
      ubahItemKeranjang(("Ubah Produk"))
      hapusItemKeranjang(("Hapus Produk"))
      
      hitungTotal(("Menghitung Total Pembayaran"))
      prosesBayar(("Memproses Pembayaran"))
      pilihMetode(("Memilih Metode Pembayaran"))
      hitungKembalian(("Menghitung Kembalian"))
      simpanRiwayat(("Menyimpan Riwayat Transaksi/Pembayaran"))
      
      tampilStruk(("Menampilkan Struk"))
      cetakStruk(("Mencetak Struk"))
    end

    subgraph ManajerScope ["Ruang Manajer (Decision Support)"]
      lihatProduk(("Melihat Produk"))
      tambahProduk(("Tambah Produk"))
      updateProduk(("Update/Edit Produk"))
      hapusProduk(("Hapus Produk"))

      lihatPromosi(("Melihat Promosi"))
      tambahPromosi(("Tambah Promosi"))
      hapusPromosi(("Hapus Promosi"))

      lihatAnalisis(("Melihat Analisis Penjualan"))
      lihatRincian(("Melihat Rincian Produk"))
      lihatOmset(("Melihat Total Omset"))
      lihatJumlahTerjual(("Melihat Jumlah Produk Terjual"))
      klasifikasiProduk(("Mengklasifikasikan Produk"))
    end
  end

  kasir --- login
  manajer --- login

  kasir --- bayarProduk
  kasir --- bayarTagihan
  kasir --- riwayatTrx
  kasir --- kelolaKeranjang
  
  kelolaKeranjang -.->|<<extend>>| tambahItemKeranjang
  kelolaKeranjang -.->|<<extend>>| ubahItemKeranjang
  kelolaKeranjang -.->|<<extend>>| hapusItemKeranjang
  
  bayarProduk --> hitungTotal
  hitungTotal -.->|<<include>>| prosesBayar
  prosesBayar -.->|<<include>>| pilihMetode
  prosesBayar -.->|<<include>>| hitungKembalian
  prosesBayar -.->|<<include>>| simpanRiwayat
  prosesBayar --> tampilStruk
  tampilStruk -.->|<<include>>| cetakStruk

  manajer --- lihatProduk
  lihatProduk -.->|<<extend>>| tambahProduk
  lihatProduk -.->|<<extend>>| updateProduk
  lihatProduk -.->|<<extend>>| hapusProduk

  manajer --- lihatPromosi
  lihatPromosi -.->|<<extend>>| tambahPromosi
  lihatPromosi -.->|<<extend>>| hapusPromosi

  manajer --- lihatAnalisis
  lihatAnalisis -.->|<<include>>| lihatRincian
  lihatAnalisis -.->|<<include>>| lihatOmset
  lihatAnalisis -.->|<<include>>| lihatJumlahTerjual
  lihatAnalisis -.->|<<include>>| klasifikasiProduk
```

<p align="center">
  <img src="docs/gambar/perancangan/Use%20case.drawio.png" alt="Use Case Diagram" width="800"/>
  <br/><em>Diagram alur interaksi use case aktor Kasir dan Manajer</em>
</p>

| Aktor | Use Case Utama | Hubungan / Relasi (Include & Extend) | Deskripsi Fungsional |
|---|---|---|---|
| **Kasir & Manajer** | `Login` | Akses Utama | Verifikasi kredensial akun dan membuka ruang kerja sesuai role. |
| **Kasir** | `Pembayaran Produk` | `-->` `Menghitung Total Pembayaran`<br/>`..> <<include>>` `Memproses Pembayaran`<br/>`..> <<include>>` `Cetak Struk` | Melayani transaksi belanja, input barcode, kalkulasi diskon FIFO, hitung kembalian, dan terbit struk. |
| **Kasir** | `Kelola Keranjang` | `..> <<extend>>` `Tambah Produk`<br/>`..> <<extend>>` `Ubah Produk`<br/>`..> <<extend>>` `Hapus Produk` | Mengatur item barang belanjaan sebelum diproses ke pembayaran. |
| **Kasir** | `Pembayaran Tagihan` | Terhubung ke Transaksi | Melayani tagihan rutin (listrik PLN, air PDAM, pulsa telko, BPJS) + biaya admin Rp2.500. |
| **Kasir** | `Melihat Riwayat Transaksi` | Query ke Transaksi | Membuka daftar transaksi lampau dan mencetak ulang struk kasir. |
| **Manajer** | `Melihat Produk` | `..> <<extend>>` `Tambah Produk`<br/>`..> <<extend>>` `Update/Edit Produk`<br/>`..> <<extend>>` `Hapus Produk` | Manajemen data master produk dan pemantauan ketersediaan stok batch. |
| **Manajer** | `Melihat Promosi` | `..> <<extend>>` `Tambah Promosi`<br/>`..> <<extend>>` `Hapus Promosi` | Manajemen kampanye diskon bertarget dan penautan ke batch mendekati expired. |
| **Manajer** | `Melihat Analisis Penjualan` | `..> <<include>>` `Melihat Rincian Produk`<br/>`..> <<include>>` `Melihat Total Omset`<br/>`..> <<include>>` `Melihat Jumlah Terjual`<br/>`..> <<include>>` `Mengklasifikasikan Produk` | Dasbor evaluasi performa bisnis: omzet harian, efektivitas promosi, dan pelabelan kinerja barang. |

</details>

---

### 3. 🗄️ Entity Relationship Diagram (ERD Logical & Relational)

Perancangan basis data `db_flatsmart` dibagi menjadi dua model: **ERD Logical** untuk melihat relasi konseptual bisnis antar entitas, dan **ERD Relational** untuk melihat implementasi fisik tabel, foreign key, dan tipe datanya.

<details open>
<summary><b>🔍 A. Model 1: ERD Logical (Model Konseptual)</b></summary>
<br/>

Model Logical berfokus pada hubungan konseptual antara entitas bisnis minimarket tanpa dibebani detail implementasi database fisik:
- **Pengguna**: Entitas induk yang membedakan aktor kasir dan manajer.
- **Produk & Stok**: Satu produk dapat memiliki banyak *batch persediaan* (1:N), di mana tanggal expired dicatat per batch stok.
- **Promosi**: Entitas diskon yang menargetkan batch stok spesifik agar promosi tepat sasaran.
- **Transaksi**: Entitas *supertype* yang memiliki dua *subclass* terpisah: transaksi penjualan produk kasir dan transaksi pembayaran tagihan (PPOB).
- **Detail Transaksi**: Entitas asosiasi yang mencatat rincian kuantitas, harga, dan subtotal dari setiap batch stok yang terjual.

<p align="center">
  <img src="docs/gambar/perancangan/logical.png" alt="ERD Logical" width="800"/>
  <br/><em>Pemodelan konseptual relasi entitas bisnis FlatSmart (ERD Logical)</em>
</p>

</details>

<br/>

<details open>
<summary><b>🔍 B. Model 2: ERD Relational (Model Fisik Relasional)</b></summary>
<br/>

Model Relational memetakan struktur database secara presisi lengkap dengan *Primary Key (PK)*, *Foreign Key (FK)*, constraint relasi, dan tipe data:

```mermaid
erDiagram
  pengguna ||--o{ transaksi : "melayani / menangani (1:N)"
  pengguna ||--o{ produk : "mengelola / mencatat (1:N)"
  pengguna ||--o{ promosi : "membuat / mengelola (1:N)"
  transaksi ||--|| transaksi_produk : "subtype transaksi penjualan (1:1)"
  transaksi ||--|| transaksi_tagihan : "subtype transaksi pembayaran (1:1)"
  transaksi_produk ||--o{ detail_transaksi : "memiliki rincian item (1:N)"
  produk ||--o{ stok : "memiliki persediaan batch (1:N)"
  promosi ||--o{ stok : "diterapkan pada batch (1:N)"
  stok ||--o{ detail_transaksi : "dirujuk pada penjualan (1:N)"

  pengguna {
    varchar username PK
    varchar password
    varchar nama_pengguna
    enum role "kasir / manajer"
  }
  produk {
    varchar barcode PK
    varchar nama
    decimal harga_beli
    decimal harga_jual
    int stok
    varchar username FK "pengguna.username"
  }
  promosi {
    varchar kode_promosi PK
    varchar nama
    decimal diskon
    datetime tanggal_mulai
    datetime tanggal_selesai
    varchar username FK "pengguna.username"
  }
  stok {
    varchar id_stok PK
    int stok
    date tanggal_exp
    varchar kode_promosi FK "promosi.kode_promosi"
    varchar barcode FK "produk.barcode"
  }
  transaksi {
    int id_transaksi PK
    varchar metode_pembayaran
    decimal total_bayar
    decimal uang_diterima
    decimal kembalian
    varchar username FK "pengguna.username"
    datetime tanggal_transaksi
  }
  transaksi_produk {
    int id_transaksi PK_FK "transaksi.id_transaksi"
    int jumlah_item
  }
  transaksi_tagihan {
    int id_transaksi PK_FK "transaksi.id_transaksi"
    varchar jenis_tagihan
    varchar no_pelanggan
    varchar nama_pelanggan
    decimal nominal_tagihan
    varchar provider
  }
  detail_transaksi {
    int id_detail_transaksi PK
    int jumlah
    decimal harga_satuan
    decimal subtotal
    int id_transaksi FK "transaksi_produk.id_transaksi"
    varchar id_stok FK "stok.id_stok"
  }
```

<p align="center">
  <img src="docs/gambar/perancangan/relational.png" alt="ERD Relational" width="800"/>
  <br/><em>Pemodelan fisik relasional basis data db_flatsmart (ERD Relational)</em>
</p>

#### Pembagian Relasi & Kardinalitas Entitas
| No | Pasangan Relasi Entitas | Kardinalitas | Penjelasan Makna Relasi |
|:---:|---|:---:|---|
| 1 | **Pengguna & Transaksi** | **One to many (1:N)** | Satu pengguna dapat melayani banyak transaksi, dan setiap transaksi dilayani oleh tepat satu pengguna. |
| 2 | **Pengguna & Produk** | **One to many (1:N)** | Satu pengguna dapat mencatat dan mengelola banyak produk, setiap produk dikelola oleh satu pengguna. |
| 3 | **Pengguna & Promosi** | **One to many (1:N)** | Satu pengguna (manajer) dapat membuat banyak promosi, setiap promosi dikaitkan dengan satu pengguna. |
| 4 | **Transaksi & Transaksi Produk** | **One to one (1:1)** | Hubungan Superclass-Subclass: satu transaksi memiliki tepat satu data rincian transaksi produk. |
| 5 | **Transaksi & Transaksi Tagihan** | **One to one (1:1)** | Hubungan Superclass-Subclass: satu transaksi memiliki tepat satu catatan transaksi tagihan PPOB. |
| 6 | **Transaksi Produk & Detail Transaksi** | **One to many (1:N)** | Satu transaksi produk memiliki banyak baris item belanja, tiap detail mengacu ke satu transaksi produk. |
| 7 | **Produk & Stok** | **One to many (1:N)** | Satu produk memiliki banyak batch stok persediaan, setiap record stok mengacu pada satu produk. |
| 8 | **Promosi & Stok** | **One to many (1:N)** | Satu program promosi dapat diterapkan pada banyak batch stok barang, tiap batch terikat satu promosi. |
| 9 | **Stok & Detail Transaksi** | **One to many (1:N)** | Satu batch stok dapat dirujuk oleh banyak baris transaksi penjualan yang telah terjadi. |

---

#### 9 Aturan ERDish Resmi
1. **ERDish Pengguna dengan Transaksi**:  
   * Setiap pengguna dapat melayani satu atau banyak transaksi.  
   * Setiap transaksi harus dilayani oleh satu dan hanya satu pengguna.
2. **ERDish Pengguna dengan Produk**:  
   * Setiap pengguna dapat mengelola satu atau banyak produk.  
   * Setiap produk harus dikelola satu dan hanya satu pengguna.
3. **ERDish Pengguna dengan Promosi**:  
   * Setiap pengguna dapat membuat satu atau banyak promosi.  
   * Setiap promosi harus dibuat oleh satu dan hanya satu pengguna.
4. **ERDish Transaksi dengan Transaksi Produk**:  
   * Setiap transaksi dapat memiliki satu dan hanya satu transaksi produk.  
   * Setiap transaksi produk harus berasal dari satu dan hanya satu transaksi.
5. **ERDish Transaksi dengan Transaksi Tagihan**:  
   * Setiap transaksi dapat memiliki satu dan hanya satu transaksi tagihan.  
   * Setiap transaksi tagihan harus berasal dari satu dan hanya satu transaksi.
6. **ERDish Transaksi Produk dengan Detail Transaksi**:  
   * Setiap transaksi produk harus memiliki satu atau banyak detail transaksi.  
   * Setiap detail transaksi harus dimiliki oleh satu dan hanya satu transaksi produk.
7. **ERDish Produk dengan Stok**:  
   * Setiap produk harus memiliki satu atau banyak stok.  
   * Setiap stok dapat dimiliki satu dan hanya satu produk.
8. **ERDish Promosi dengan Stok**:  
   * Setiap promosi dapat menerapkan satu atau banyak stok.  
   * Setiap stok harus diterapkan satu dan hanya satu promosi.
9. **ERDish Stok dengan Detail Transaksi**:  
   * Setiap stok harus memiliki satu atau banyak detail transaksi.  
   * Setiap detail transaksi harus dimiliki oleh satu dan hanya satu stok.

</details>

---

<a id="-struktur-folder--package"></a>
## 📁 Struktur Folder / Package

```text
flatsmart/
├── pom.xml                         # Konfigurasi Maven (Java 17, Driver MySQL 9.4.0)
├── nbactions.xml                   # Runner Script NetBeans (exec-maven-plugin)
├── db_flatsmart.sql                # Skema DDL & Data Dummy Lengkap (8 Tabel)
├── lib/                            # Pustaka lokal (AbsoluteLayout SNAPSHOT)
├── docs/                           # Dokumentasi Arsitektur, Flowchart, Use-Case & Gambar
│   ├── arsitektur.md
│   ├── flowchart.md
│   ├── use-case.md
│   └── gambar/                     # Aset Screenshot Presentasi README
└── src/main/
    ├── java/
    │   ├── com/mycompany/flatsmart/
    │   │   └── Flatsmart.java      # Main Entry Point (Pemeriksaan DB & Inisialisasi GUI)
    │   ├── view/                   # [VIEW] 14 Layar Swing Form (.java & .form)
    │   ├── controller/             # [CONTROLLER] 11 Controller & Kontrak Interface
    │   ├── service/                # [SERVICE] 8 Business Logic Services & Atomic Handler
    │   ├── dao/                    # [DAO] 6 Data Access Objects (Native SQL Builder)
    │   ├── model/                  # [MODEL] 10 POJO / Entity DTO
    │   ├── config/                 # [CONFIG] DatabaseConnection (Singleton Pool Engine)
    │   └── util/                   # [UTIL] ExcelWriter, Format, Regex, DatePicker
    └── resources/
        └── icons/                  # 24 Aset Ikon Antarmuka High-Resolution (.png)
```

<div align="center">

| Package | Jumlah Kelas | Tanggung Jawab Utama | Prinsip Pemisahan Tugas |
|---|:---:|---|---|
| `view` | 14 (+14 `.form`) | Menampilkan komponen visual, menangkap interaksi pengguna, merender tabel dan grafik. | **Bebas dari sintaks SQL dan JDBC.** |
| `controller` | 11 | Menjadi jembatan antara View dan Service; memvalidasi parameter dasar. | Menegakkan kontrak antarmuka CRUD seragam. |
| `service` | 8 | Mengatur logika bisnis minimarket: FIFO, diskon bertarget, dan pembungkusan transaksi. | Menjamin atomisitas commit/rollback multi-tabel. |
| `dao` | 6 | Menulis klausa kueri SQL dan memetakan `ResultSet` JDBC menjadi objek Model. | **Satu-satunya pemilik kalimat SQL.** |
| `model` | 10 | Representasi entitas data dengan atribut `private` dan *getter/setter*. | Mengamankan integritas nilai data (*State Isolation*). |
| `config` | 1 | Mengelola kolam koneksi (*Connection Pool*), siklus hidup koneksi, dan thread safety. | Menerapkan Singleton Pattern anti-kebocoran koneksi. |
| `util` | 8 | Kelas bantu: generator Excel `.xlsx`, pemformat Rupiah, validator regex, kalender popup. | Modular dan dapat digunakan ulang di seluruh layar. |

</div>

---

<a id="-penjelasan-penerapan-4-pilar-oop-di-dalam-program"></a>
## 🎯 Penjelasan Penerapan 4 Pilar OOP di dalam Program

Proyek FlatSmart dibangun dengan menerapkan **4 Pilar Utama Pemrograman Berorientasi Objek (OOP)** secara menyeluruh untuk menjamin keterbacaan, keamanan data, dan kemudahan pemeliharaan:

<br/>

### 1. 🛡️ Encapsulation (Enkapsulasi)
Semua atribut dalam kelas model dan konfigurasi diatur dengan hak akses `private`. Akses dan manipulasi nilai hanya dapat dilakukan melalui metode *getter* dan *setter*. Logika perhitungan internal dibungkus rapat di dalam kelasnya tanpa memaparkan data mentah.

Contoh implementasi enkapsulasi pada kelas Model:
```java
public class Promosi {
    private String kodePromosi;
    private String namaPromosi;
    private LocalDate tglMulai;
    private LocalDate tglSelesai;

    public String getStatus() {
        LocalDate now = LocalDate.now();
        if (now.isBefore(tglMulai))  return "Akan datang";
        if (now.isAfter(tglSelesai)) return "Berakhir";
        return "Aktif";
    }
}
```
* **Penjelasan & Kegunaan**: Status promosi tidak disimpan sebagai nilai string statis di database, melainkan dihitung secara dinamis melalui metode `getStatus()`. Atribut `tglMulai` dan `tglSelesai` dienkapsulasi rapat sehingga objek View tidak dapat mengubah tanggal secara langsung. Kredensial JDBC pada kelas `DatabaseConnection` juga dienkapsulasi dengan modifier `private` agar alamat host, username, dan password database tidak bocor keluar kelas.

---

### 2. 🧬 Inheritance (Pewarisan)
Mewariskan atribut dan metode umum dari superclass ke subclass untuk mencegah duplikasi kode (*Don't Repeat Yourself*).

Contoh implementasi pewarisan pada Controller:
```java
public abstract class BasisController {
    private final String modul;

    protected BasisController(String modul) { this.modul = modul; }
    public final String modul() { return modul; }

    protected String idWajib(String id) {
        if (id == null || id.isBlank()) {
            throw new IllegalArgumentException(modul + ": data yang dipilih tidak valid.");
        }
        return id.trim();
    }
}

public class ProdukController extends BasisController implements CrudController<Produk> {
    private final ProdukService service = new ProdukService();

    public ProdukController() {
        super("Produk");
    }

    @Override
    public void hapus(String barcode) throws SQLException {
        service.hapus(idWajib(barcode));
    }
}
```
* **Penjelasan & Kegunaan**: Kelas `ProdukController` mewarisi `BasisController`. Dengan memanggil `super("Produk")`, subclass otomatis mewarisi identitas nama modul serta metode validasi `idWajib()`. Jika format validasi ID perlu diubah di kemudian hari, pengembang cukup memperbarui logika di kelas induk `BasisController` dan seluruh controller turunan otomatis terbarui.

---

### 3. 🎭 Polymorphism (Polimorfisme)
Kemampuan suatu objek atau metode untuk memiliki banyak bentuk melalui **Interface Polymorphism**, **Method Overriding**, dan **Functional Interface (Lambdas)**.

Contoh implementasi polimorfisme interface dan functional callback:
```java
private final CrudController<Produk> controller = new ProdukController();

@FunctionalInterface
public interface PsWork<T> { T run(PreparedStatement ps) throws SQLException; }

return DatabaseConnection.query(SQL_CARI_BARCODE, ps -> {
    ps.setString(1, barcode);
    try (ResultSet rs = ps.executeQuery()) {
        return rs.next() ? peta(rs) : null;
    }
});
```
* **Penjelasan & Kegunaan**: Form antarmuka memanggil kontrak interface `CrudController<Produk>`, bukan kelas konkretnya secara langsung. Selain itu, metode `DatabaseConnection.query()` memanfaatkan functional interface `PsWork<T>` sehingga berbagai query SQL dari berbagai DAO dapat dieksekusi dengan bentuk pemanggilan seragam menggunakan ekspresi lambda.

---

### 4. 🧩 Abstraction (Abstraksi)
Menyembunyikan detail implementasi teknis yang rumit dan hanya memperlihatkan antarmuka esensial kepada pengguna kelas.

Contoh kontrak abstraksi dan transaksi atomik:
```java
public interface CrudController<T> extends BacaController<T> {
    List<T> semua() throws SQLException;
    void tambah(T entity) throws SQLException;
    void ubah(T entity) throws SQLException;
    void hapus(String id) throws SQLException;
}

@FunctionalInterface public interface SqlWork<T> { T run() throws SQLException; }

public static <T> T transaction(SqlWork<T> work) throws SQLException {
    Connection c = ambilKoneksiTransaksi();
    boolean komit = false;
    try {
        T res = work.run();
        c.commit();
        komit = true;
        return res;
    } finally {
        if (!komit) c.rollback();
    }
}
```
* **Penjelasan & Kegunaan**: Lapisan View sama sekali tidak mengetahui sintaks query SQL, driver JDBC, maupun proses buka-tutup koneksi. View cukup memanggil antarmuka tingkat tinggi seperti `PenjualanController.proses()`. Seluruh kerumitan `setAutoCommit(false)`, `commit()`, dan `rollback()` disembunyikan di dalam lapisan abstraksi `DatabaseConnection.transaction()`.

---

<a id="️-cara-penggunaan-program-sertakan-screenshot-gui"></a>
## ▶️ Cara Penggunaan Program (Sertakan Screenshot GUI)

### 1. Persiapan Lingkungan & Instalasi

| Langkah | Instruksi Instalasi | Tampilan / Screenshot |
|:---:|---|:---:|
| **1** | Nyalakan service **MySQL & Apache** melalui **Laragon** atau XAMPP pada port default `3306`. | <img src="docs/gambar/penggunaan/Laragon.png" alt="Laragon Server" width="280"/> |
| **2** | Buat database `db_flatsmart` dan import berkas `db_flatsmart.sql` lewat phpMyAdmin atau terminal. | <img src="docs/gambar/penggunaan/Import%20Database.png" alt="Import Database" width="280"/> |
| **3** | Buka project FlatSmart di **Apache NetBeans** (`File > Open Project`), tunggu Maven memuat dependensi otomatis. | <img src="docs/gambar/penggunaan/Open%20Project.png" alt="Buka Project NetBeans" width="280"/> |
| **4** | Klik kanan pada project di NetBeans ➡️ pilih **Run** (atau tekan **F6**). Konfigurasi `nbactions.xml` akan mengompilasi dan membuka `LoginFrame`. | <img src="docs/gambar/penggunaan/Run.png" alt="Run NetBeans" width="280"/> |
| **5** | Jika koneksi database belum menyala, sistem akan menampilkan dialog peringatan koneksi sebelum keluar. | <img src="docs/gambar/penggunaan/Login%20Error.png" alt="Error Koneksi" width="280"/> |

---

### 2. Akun Demo Bawaan Database

Sistem telah menyediakan akun demo siap pakai yang tersimpan di tabel `pengguna`:

| Hak Akses | Username | Password | Nama Pengguna | Akses Menu |
|:---:|:---:|:---:|---|---|
| **Kasir** | `ksr01` | *tercatat di SQL* | Andi Pratama | Penjualan, Tagihan PPOB, Riwayat Transaksi |
| **Kasir** | `ksr02` | *tercatat di SQL* | Dina Marlina | Penjualan, Tagihan PPOB, Riwayat Transaksi |
| **Kasir** | `ksr03` | *tercatat di SQL* | Fajar Nugroho | Penjualan, Tagihan PPOB, Riwayat Transaksi |
| **Manajer** | `mgr01` | *tercatat di SQL* | Rina Wulandari | Kelola Produk, Promosi Diskon, Dasbor Analisis, Export Excel |

---

### 3. Panduan Alur Kerja Kasir (Front Office)

| No | Tahapan Transaksi | Penjelasan Alur | Screenshot Antarmuka |
|:---:|---|---|:---:|
| **1** | **Login Akun Kasir** | Masukkan username `ksr01` dan password. Sistem membuka ruang kerja kasir. | <img src="docs/gambar/penggunaan/Home%20Kasir.png" alt="Home Kasir" width="280"/> |
| **2** | **Input Keranjang Belanja** | Scan barcode atau ketik nama produk. Batch kedaluwarsa terdekat & promo otomatis terpasang. | <img src="docs/gambar/penggunaan/Kasir%20Keranjang.png" alt="Keranjang" width="280"/> |
| **3** | **Proses Pembayaran & Konfirmasi Transaksi** | Pilih metode bayar (Tunai/QRIS/Debit), input uang diterima, dan konfirmasi. Header, detail belanja, dan pengurangan stok tersimpan atomik. Struk 40-kolom siap dicetak. | <img src="docs/gambar/penggunaan/Pembayaran.png" alt="Pembayaran" width="240"/><br/><img src="docs/gambar/penggunaan/Struk.png" alt="Struk Kasir" width="240"/><br/><img src="docs/gambar/penggunaan/Cetak%20struk.png" alt="Cetak Struk" width="240"/> |
| **4** | **Pembayaran Tagihan PPOB** | Buka menu Tagihan, input ID pelanggan dan nominal. Biaya admin Rp2.500 otomatis ditambahkan. | <img src="docs/gambar/penggunaan/Pembayaran%20tagihan.png" alt="Tagihan" width="280"/> |
| **5** | **Pencarian Riwayat Transaksi** | Buka menu Riwayat untuk melihat transaksi kasir lampau atau mencetak ulang struk lama. | <img src="docs/gambar/penggunaan/Lihat%20transaksi.png" alt="Riwayat" width="280"/> |

---

### 4. Panduan Alur Kerja Manajer (Back Office)

| No | Tahapan Manajerial | Penjelasan Alur | Screenshot Antarmuka |
|:---:|---|---|:---:|
| **1** | **Login Akun Manajer** | Masukkan username `mgr01`. Sistem membuka `ManajerFrame` pada panel Kelola Produk. | <img src="docs/gambar/penggunaan/Home%20Manajer.png" alt="Produk" width="280"/> |
| **2** | **Tambah Produk Baru** | Isi barcode, nama, harga beli, harga jual, stok awal, dan tanggal expired batch pertama. | <img src="docs/gambar/penggunaan/Tambah%20produk.png" alt="Form Tambah Produk" width="280"/> |
| **3** | **Perbarui Data Produk** | Ubah data master harga beli dan harga jual produk yang sudah tersimpan di database. | <img src="docs/gambar/penggunaan/Update%20produk.png" alt="Update Produk" width="280"/> |
| **4** | **Hapus Produk** | Penghapusan data master produk. Sistem otomatis menolak bila produk pernah ditransaksikan. | <img src="docs/gambar/penggunaan/Hapus%20produk.png" alt="Hapus Produk" width="280"/> |
| **5** | **Inspeksi Batch Stok** | Klik baris produk untuk menampilkan rincian ID batch, kuantitas, dan tanggal expired di bawah tabel. | <img src="docs/gambar/penggunaan/Batch%20produk.png" alt="Batch" width="280"/> |
| **6** | **Kelola Promosi Diskon** | Masukkan nama promo, tentukan diskon persen, periode tanggal, dan kaitkan ke batch target. | <img src="docs/gambar/penggunaan/Tambah%20Promosi.png" alt="Promosi" width="280"/> |
| **7** | **Analisis Penjualan & KPI** | Tentukan rentang tanggal analisis, klik Tampilkan untuk melihat KPI, omzet, dan grafik batang. | <img src="docs/gambar/penggunaan/Analisis%20penjualan.png" alt="Analisis" width="280"/> |
| **8** | **Tinjau Rekomendasi Diskon**| Klik tombol tinjau pada batch yang mendekati expired untuk langsung meluncurkan promo. | <img src="docs/gambar/penggunaan/Tinjauan%20diskon.png" alt="Tinjau Diskon" width="280"/> |
| **9** | **Drill-Down Detail Barang** | Klik-ganda baris produk di tabel analisis untuk membuka riwayat transaksi lengkap barang itu. | <img src="docs/gambar/penggunaan/Detail%20produk.png" alt="Detail Produk" width="280"/> |
| **10** | **Ekspor Laporan Excel** | Klik tombol Export Excel untuk menyimpan laporan analisis 4-sheet dalam format `.xlsx`. | <img src="docs/gambar/penggunaan/Export%20excel.png" alt="Export Excel" width="280"/> |

---

<a id="-kontributor-nama-dan-nim"></a>
## 👥 Kontributor (Nama dan NIM)

Proyek ini dikembangkan oleh tim mahasiswa **Program Studi Sistem Informasi, Fakultas Teknik, Universitas Mulawarman (2026)**:

<div align="center">

| Foto / Avatar | Nama Lengkap | NIM | Pembagian Peran & Job Deskripsi |
|:---:|---|:---:|---|
| <img src="https://api.dicebear.com/7.x/bottts/svg?seed=Fajar" width="65"/> | **AHMAD FAJAR NOVIA** | `2509116041` | **Lead Software Architect & Full-Stack Developer**<br/>• Perancangan konsep sistem, arsitektur 5-Layer MVC, DAO Pattern, dan Singleton Connection Pool.<br/>• Pengembangan seluruh *source code* aplikasi Java Swing (Kasir & Manajer) di Apache NetBeans.<br/>• Perancangan dan pembuatan skema basis data awal MySQL (`CREATE TABLE`, constraint, & `INSERT` data awal).<br/>• Perancangan 5 Flowchart alur kerja sistem dan penyusunan dokumentasi komprehensif README.md. |
| <img src="https://api.dicebear.com/7.x/bottts/svg?seed=Farah" width="65"/> | **FARAH HIKMATUL MAULA** | `2509116099` | **Database Query Specialist & Documentation Lead**<br/>• Penyusunan dan penulisan dokumen resmi Laporan Project Akhir Praktikum Sistem Basis Data.<br/>• Perancangan materi presentasi (PPT) pemodelan ERD dan basis data relasional.<br/>• Implementasi kueri SQL relasional: DDL, DML, operasi `JOIN` multi-tabel, dan kueri *Select Tingkat Lanjut 1*. |
| <img src="https://api.dicebear.com/7.x/bottts/svg?seed=Marza" width="65"/> | **MARZA HANAYA MELODYA GOGA** | `2409116103` | **Database Analyst & Presentation Specialist**<br/>• Perancangan dan penyusunan materi presentasi (PPT) untuk pemodelan ERD (Logical & Relational).<br/>• Analisis kebutuhan sistem basis data, validasi kardinalitas entitas, dan aturan ERDish.<br/>• Perancangan kueri analisis data: agregasi penjualan, kalkulasi performa, dan kueri *Select Tingkat Lanjut 2*. |
| <img src="https://api.dicebear.com/7.x/bottts/svg?seed=Harits" width="65"/> | **HARITS** | `2509116048` | **Associate Developer & Modeling Specialist**<br/>• Perancangan Use Case Diagram dan materi presentasi (PPT) skenario aktor sistem.<br/>• Kontribusi pendukung dalam pengembangan kode program dan pengujian fungsional aplikasi.<br/>• Penyusunan dokumentasi use case dan analisis interaksi antarmuka pengguna. |

</div>

<br/>

> 🎓 **Afiliasi**: Program Studi Sistem Informasi • Fakultas Teknik • Universitas Mulawarman (2026)

---

## 📎 Dokumen Referensi & Lampiran

- 📐 **Dokumen Arsitektur Lengkap**: [`docs/arsitektur.md`](docs/arsitektur.md)
- 📊 **Source Flowchart (Mermaid Source)**: [`docs/flowchart.md`](docs/flowchart.md)
- 👤 **Dokumentasi Skenario Use Case**: [`docs/use-case.md`](docs/use-case.md)
- 🗄️ **Skema Basis Data DDL & DML**: [`db_flatsmart.sql`](db_flatsmart.sql)
- 🖼️ **Daftar Lengkap Aset Gambar README**: [`docs/gambar/README.md`](docs/gambar/README.md)

<div align="center">
  <br/>
  <b>FlatSmart v1.0 — Capstone Pemrograman Berorientasi Objek & Praktikum Sistem Basis Data</b><br/>
  <i>Developed with Java 17, Apache NetBeans, Swing, MySQL, Figma, and GitHub</i>
</div>
