# Dashboard Climate Change R

## Sekilas tentang Proyek ini

Perubahan iklim berdampak besar terhadap peningkatan frekuensi dan intensitas bencana hidrometeorologi di Indonesia, seperti banjir, kekeringan, dan angin kencang. Fenomena ini bukan lagi kejadian luar biasa, melainkan pola baru yang makin kompleks dan meluas dampaknya.

Statistik lingkungan berperan penting dalam menyusun kebijakan adaptasi dan mitigasi. Indonesia, sebagai negara kepulauan, sangat rentan terhadap krisis iklim yang mengancam aspek sosial, ekonomi, hingga kesehatan. BNPB mencatat tingginya kejadian bencana pada 2020–2024, menandakan urgensi akses data yang cepat dan terintegrasi.

Dashboard ini hadir untuk menjawab kebutuhan tersebut, menyajikan data korban bencana terkait perubahan iklim secara interaktif agar dapat digunakan sebagai dasar pengambilan keputusan yang tepat dan berbasis bukti.




## Cara Memakai

[Dashboard dapat diakses secara online](https://asyarimuchtari.shinyapps.io/Dashboard_Climate_Change)

Atau anda bisa menjalankan nya sendiri jika memiliki R. Untuk dapat menjalankan dashboard ini terdapat beberapa library yang harus diinstall.

```r
install.packages(c("shiny","bs4dash","readxl","dplyr","DT","plotly","GGally","ggplot2","broom","tidyverse","sf","leaflet","car","lmtest","here"))
```

lalu jalankan Dashboard Climate.R


## Dataset

Data iklim diambil menggunakan API NASA yang sudah terintegrasi pada library R, menggunakan library [nasapower](https://github.com/ropensci/nasapower)

Data bencana diambil dari [dashboard bencana](https://dibi.bnpb.go.id/superset/dashboard/2/) Badan Nasional Penanggulangan Bencana (BNPB)

Anda bisa melakukan perluasan dari dataset yang kami gunakan pada tautan diatas, atau gunakan dataset kami langsung yang sudah tertera pada main branch.


## Authors

- [Dinda Putri Nur Wulandari](https://github.com/dindapnw)
- [Muhammad Hamlul Khair](https://github.com/hamlulkhair)
- [Qurany Nadhira Tsabita](https://github.com/lazydoughnut)
- [T.M. Al-Asy'ari Al-Muchtari](https://github.com/SeraphimeZelel)
- [Wahyu Nugraha Raomi Gading](https://github.com/wahyugading)

