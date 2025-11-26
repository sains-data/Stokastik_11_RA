# Analisis Pola Transisi Platform Informasi Kampus Menggunakan Rantai Markov

**Studi Kasus: Program Studi Sains Data, Institut Teknologi Sumatera (ITERA)**

## Gambaran Umum

Proyek ini merupakan laporan penelitian yang menerapkan metode Pemodelan Stokastik, khususnya Rantai Markov (Markov Chain), untuk menganalisis perilaku mahasiswa dalam mengakses informasi kampus. Penelitian ini memodelkan pola perpindahan (switching behavior) mahasiswa antar tiga platform utama: Instagram, WhatsApp, dan Website Kampus.

Tujuan utama dari analisis ini adalah untuk menentukan platform mana yang menjadi pusat aktivitas jangka panjang (steady state) dan memberikan rekomendasi strategi penyebaran informasi yang lebih efektif bagi manajemen program studi.

## Tim Peneliti (Kelompok 11)

Proyek ini disusun oleh mahasiswa Program Studi Sains Data ITERA:

* **Dea Mutia Risani** (122450099)
* **Rian Bintang Wijaya** (122450094)
* **Uliano Wilyam Purba** (122450098)
* **Baruna Abirawa** (122450097)

## Latar Belakang Masalah

Program Studi Sains Data ITERA memanfaatkan berbagai saluran media untuk menyebarkan informasi akademik. Namun, penggunaan multi-platform menyebabkan fokus mahasiswa terpecah. Pola perpindahan mahasiswa antar platform (misalnya dari Website ke Instagram atau sebaliknya) bersifat stokastik atau acak.

Oleh karena itu, diperlukan model matematika untuk memprediksi probabilitas perpindahan dan kondisi keseimbangan (steady state) di masa depan guna mengevaluasi efektivitas masing-masing platform.

## Metodologi

Penelitian ini menggunakan pendekatan kuantitatif dengan rincian sebagai berikut:

* **Metode:** Rantai Markov Waktu Diskrit (Discrete Time Markov Chain).
* **Data:** Data primer dari survei terhadap 81 responden mahasiswa aktif.
* **Variabel (State):**
    1.  Instagram
    2.  WhatsApp
    3.  Website Kampus
* **Analisis:** Pembentukan Matriks Frekuensi, Matriks Probabilitas Transisi, dan Perhitungan Distribusi Steady State.

## Hasil Analisis

### 1. Matriks Probabilitas Transisi (Satu Langkah)

Tabel berikut menunjukkan peluang perpindahan pengguna dari satu platform (baris) ke platform lain (kolom) dalam satu langkah waktu:

| Dari/Ke | Instagram | WhatsApp | Website Kampus |
| :--- | :--- | :--- | :--- |
| **Instagram** | 0.00 | 0.53 | 0.47 |
| **WhatsApp** | 0.70 | 0.00 | 0.30 |
| **Website** | 0.65 | 0.35 | 0.00 |

*Catatan: Instagram menerima perpindahan tertinggi dari WhatsApp (0.70) dan Website (0.65).*

### 2. Analisis Steady State (Jangka Panjang)

Berdasarkan simulasi hingga mencapai kondisi keseimbangan (konvergen), diperoleh distribusi probabilitas jangka panjang sebagai berikut:

| Peringkat | Platform | Probabilitas Steady State | Analisis |
| :--- | :--- | :--- | :--- |
| **1** | **Instagram** | **40.48%** | Menjadi platform paling dominan dan pusat tujuan utama informasi. |
| **2** | **WhatsApp** | **31.26%** | Berperan sebagai media pendukung dan jalur distribusi pesan cepat. |
| **3** | **Website Kampus** | **28.25%** | Memiliki retensi paling rendah dibanding platform media sosial. |

## Kesimpulan dan Rekomendasi

1.  **Instagram:** Hasil menunjukkan bahwa arus informasi kampus cenderung bermuara di Instagram. Strategi komunikasi sebaiknya memprioritaskan konten visual yang informatif di platform ini.
2.  **WhatsApp:** WhatsApp efektif sebagai "relay" atau penguat distribusi informasi karena sifatnya yang personal dan cepat.
3.  **Website Kampus:** Website Kampus memiliki tingkat kunjungan ulang (steady state) terendah. Diperlukan perbaikan antarmuka dan aksesibilitas agar kembali menjadi rujukan utama yang kompetitif.

## Referensi Utama

* Laporan Pemodelan Stokastik Kelompok 11, Sains Data ITERA (2025).
* Isaacson, D. L., & Madsen, R. W. (1976). *Markov Chains: Theory and Applications*.
* Howard, R. A. (1984). *Dynamic Probabilistic Systems, Vol. I: Markov Models*.
