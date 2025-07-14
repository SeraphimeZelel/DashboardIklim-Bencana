# Dashboard Climate Change R

![Versi Aplikasi](https://img.shields.io/badge/Versi-1.0.0-blue.svg)
![Lisensi](https://img.shields.io/badge/License-MIT-green.svg)

---

## Sekilas tentang Proyek ini

Perubahan iklim berdampak besar terhadap peningkatan frekuensi dan intensitas bencana hidrometeorologi di Indonesia, seperti banjir, kekeringan, dan angin kencang. Fenomena ini bukan lagi kejadian luar biasa, melainkan pola baru yang makin kompleks dan meluas dampaknya.

Statistik lingkungan berperan penting dalam menyusun kebijakan adaptasi dan mitigasi. Indonesia, sebagai negara kepulauan, sangat rentan terhadap krisis iklim yang mengancam aspek sosial, ekonomi, hingga kesehatan. BNPB mencatat tingginya kejadian bencana pada 2020–2024, menandakan urgensi akses data yang cepat dan terintegrasi.

Dashboard ini hadir untuk menjawab kebutuhan tersebut, menyajikan data korban bencana terkait perubahan iklim secara interaktif agar dapat digunakan sebagai dasar pengambilan keputusan yang tepat dan berbasis bukti.

---

## Fitur Utama

Aplikasi ini dilengkapi dengan berbagai fitur untuk memfasilitasi analisis data yang komprehensif:

* **📊 Dashboard Berdasarkan Provinsi dan Bencana:** Berbagai data dan jenis grafik (plot garis, plot batang, pie-chart) yang dapat disesuaikan secara dinamis oleh pengguna melalui widget input seperti Pilih Provinsi, Pilih Bencana, dan Slider Tahun.
* **🗺️ Peta Sebaran Reaktif:** Visualisasi data bencana dan iklim menggunakan peta koroplet (choropleth map) yang memungkinkan pengguna melihat sebaran data bencana atau perubahan iklim pada tiap provinsi di Indonesia.
* **📈 Analisis Korelasi dan Regresi:** Melakukan analisis inferensia secara mendalam, antar tiap variabel yang disediakan.
* **📋 Tabel Data Responsif:** Penyajian data mentah dalam format tabel interaktif yang mendukung fitur pencarian, pengurutan (sorting), dan paginasi untuk memudahkan eksplorasi data tabular.
* **🔎 Metadata:** Fitur untuk membantu pengguna memahami, mengelola, dan menggunakan data secara efektif.

---

## Library yang Digunakan

| Pustaka (Library) | Fungsi |
|---|---|
| `shiny` | Menyediakan kerangka kerja inti untuk membangun aplikasi web interaktif dengan R. |
| `bs4Dash` | Menawarkan templat dasbor Bootstrap 4 untuk aplikasi `shiny`, memperkaya antarmuka pengguna. |
| `readxl` | Memfasilitasi impor data dari file Excel (baik `.xls` maupun `.xlsx`) ke dalam R. |
| `dplyr` | Komponen inti dari `tidyverse`, menyediakan tata bahasa manipulasi data dengan fungsi untuk memfilter, memilih, mengubah, dan merangkum data. |
| `DT` | Menyediakan antarmuka ke pustaka JavaScript `DataTables`, memungkinkan pembuatan tabel interaktif di aplikasi `shiny` dan dokumen R Markdown. |
| `plotly` | Membuat grafik dan visualisasi interaktif berkualitas publikasi. |
| `GGally` | Memperluas `ggplot2` dengan menambahkan fungsi untuk membuat plot yang lebih kompleks, seperti matriks sebar (scatterplot matrices). |
| `ggplot2` | Sebuah sistem untuk membuat grafik secara deklaratif, berdasarkan "The Grammar of Graphics". Ini adalah alat fundamental untuk visualisasi data di R. |
| `broom` | Merapikan output dari fungsi bawaan R (seperti `lm`, `nls`, atau `t.test`) ke dalam format data frame yang konsisten. |
| `tidyverse` | Kumpulan paket R (termasuk `dplyr`, `ggplot2`, `readr`, `tidyr`, dll.) yang dirancang khusus untuk ilmu data. |
| `sf` | (Simple Features) Menyediakan cara standar untuk mengkodekan dan bekerja dengan data vektor spasial (titik, garis, poligon) di R. |
| `leaflet` | Antarmuka ke pustaka JavaScript `Leaflet` untuk membuat peta interaktif. |
| `car` | (Companion to Applied Regression) Menawarkan berbagai fungsi untuk pemodelan regresi, termasuk alat untuk diagnostik dan transformasi data. |
| `lmtest` | Menyediakan kumpulan tes, set data, dan contoh untuk pemeriksaan diagnostik dalam model regresi linier. |
| `here` | Menyederhanakan manajemen jalur file (file path), sehingga lebih mudah menemukan file dalam struktur direktori proyek. |
| `stringr` | Bagian dari `tidyverse`, menawarkan serangkaian fungsi yang kohesif untuk bekerja dengan teks (string). |
| `forecast` | Menyediakan metode dan alat untuk menganalisis dan meramalkan data deret waktu univariat. |
| `scales` | Mengatur pemetaan data ke atribut estetika di `ggplot2`, menyediakan alat untuk memformat sumbu dan legenda (misalnya, format koma, persentase). |
| `shinyWidgets` | Melengkapi aplikasi `shiny` dengan widget input khusus (misalnya, tombol sakelar, slider yang lebih baik, pemilih). |
| `fontawesome` | Memudahkan penyisipan ikon dari Font Awesome ke dalam dokumen R Markdown dan aplikasi `shiny`. |
| `rmarkdown` | Paket inti untuk membuat dokumen dinamis yang menggabungkan kode, output, dan teks. |
| `knitr` | Mesin serbaguna untuk pembuatan laporan dinamis di R, yang memungkinkan integrasi kode R ke dalam berbagai format output. |

---

## 🚀 Cara Memakai

[Dashboard dapat diakses secara online](https://asyarimuchtari.shinyapps.io/Dashboard_Climate_Change)

Atau ikuti langkah-langkah di bawah ini untuk menjalankan aplikasi ini di lingkungan lokal Anda.

#### 1. Prasyarat
* **Git:** Terinstal di sistem Anda untuk melakukan kloning repositori.
* **R:** Versi 4.1.0 atau lebih baru.
* **RStudio:** Versi 2022.07 atau lebih baru direkomendasikan.

#### 2. Kloning Repositori
Buka Terminal atau Git Bash, lalu jalankan perintah berikut:
```bash
git clone https://github.com/SeraphimeZelel/DashboardIklim-Bencana
cd NAMA_REPO_ANDA
```

#### 3. Install Packages

```r
install.packages(c(
  "shiny", 
  "bs4Dash", 
  "readxl", 
  "dplyr", 
  "DT", 
  "plotly", 
  "GGally", 
  "ggplot2", 
  "broom", 
  "tidyverse", 
  "sf", 
  "leaflet", 
  "car", 
  "lmtest", 
  "here", 
  "stringr", 
  "forecast", 
  "scales", 
  "shinyWidgets", 
  "fontawesome", 
  "rmarkdown", 
  "knitr"
))
```

#### 4. Menjalankan Aplikasi

Setelah semua paket terinstal dan data sudah disiapkan, buka Dashboard Climate di RStudio. Klik tombol "Run App" yang muncul di bagian atas editor untuk meluncurkan aplikasi.

---

## 📊 Sumber Data

Data yang digunakan dalam proyek ini bersumber dari berbagai institusi dan platform data publik yang kredibel.
- Data iklim diambil menggunakan API NASA yang sudah terintegrasi pada library R, menggunakan library [nasapower](https://github.com/ropensci/nasapower-)
- Data bencana diambil dari [dashboard bencana](https://dibi.bnpb.go.id/superset/dashboard/2/) Badan Nasional Penanggulangan Bencana (BNPB)

Anda bisa melakukan perluasan dari dataset yang kami gunakan pada tautan diatas, atau gunakan dataset kami langsung yang sudah tertera pada main branch.

---

## 👥 Authors

- [Dinda Putri Nur Wulandari](https://github.com/dindapnw)
- [Muhammad Hamlul Khair](https://github.com/hamlulkhair)
- [Qurany Nadhira Tsabita](https://github.com/lazydoughnut)
- [T.M. Al-Asy'ari Al-Muchtari](https://github.com/SeraphimeZelel)
- [Wahyu Nugraha Raomi Gading](https://github.com/wahyugading)

---

## 📜 Lisensi
Proyek ini dilisensikan di bawah Lisensi MIT.
Lisensi ini mengizinkan siapa saja untuk menggunakan, menyalin,
memodifikasi, dan mendistribusikan kode ini untuk tujuan apa pun, 
baik komersial maupun non-komersial, selama pemberitahuan hak cipta 
dan lisensi asli disertakan dalam semua salinan atau bagian penting dari perangkat lunak.
