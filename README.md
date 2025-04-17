# **Capstone Project Modul 2: Analisis Listing Airbnb di Bangkok**

## Latar Belakang

Dalam beberapa tahun terakhir, **Airbnb** telah menjadi pilihan utama bagi banyak wisatawan dunia. Airbnb adalah sebuah platform online yang mempertemukan **pemilik properti** (host), seperti rumah, apartemen, kamar pribadi, vila, hingga akomodasi unik lainnya dengan **penyewa** (guest) yang sedang mencari tempat tinggal fleksibel, baik untuk liburan, perjalanan bisnis, maupun keperluan pribadi lainnya.

Kalau dibandingkan dengan penginapan konvensional seperti hotel, Airbnb menawarkan fleksibilitas yang lebih tinggi. Misalnya, tamu bisa memilih tinggal di properti yang lebih “rumahan”, bisa masak sendiri, dan terasa lebih personal karena kadang tinggal satu rumah dengan host-nya. Bagi sebagian traveler, hal ini justru memberikan pengalaman yang lebih otentik. **(Sumber berita terkait perbedaan Airbnb dan Hotel : https://www.liputan6.com/hot/read/5634501/perbedaan-airbnb-dan-hotel-pada-umumnya-opsi-tempat-menginap-saat-traveling?page=2)

**Kelebihan Airbnb:**
- Harga lebih fleksibel dan kompetitif
- Pilihan properti sangat beragam dan unik
- Cocok untuk long stay maupun short stay
- Fleksibilitas dalam hal fasilitas dan durasi menginap
- Bisa merasakan kesempatan tinggal "seperti lokal"

**Kekurangannya:**
- Pada umumnya, Airbnb tidak menyediakan fasilitas seperti yang biasa ditemukan di hotel, seperti room service atau resepsionis.
- Kualitas bisa sangat bervariasi antar host
- Check-in kadang tidak sepraktis hotel jika host tidak responsif

## Cara Airbnb mendapat keuntungan:

Mengutip dari Pusat Bantuan di website Airbnb terkait Biaya dan layanan Airbnb **(Sumber: https://www.airbnb.co.id/help/article/1857?_set_bev_on_new_domain=1744561779_EAN2Y4NWU1OTEyYz)**, platform Airbnb mendapatkan keuntungan dari **komisi** yang dikenakan kepada:
- *Host*: sekitar 3% dari biaya pemesanan.
- *Guest*: sekitar 6–12% tergantung faktor lokasi dan durasi menginap.

## Target Pengguna Airbnb

Biasanya, Airbnb digunakan oleh:
- Traveler muda usia 20–40 tahun
- Digital nomad atau remote worker
- Backpacker
- Keluarga kecil yang ingin tempat lebih luas
- Pasangan atau solo traveler yang ingin suasana lokal

**Referensi terkait target pengguna Airbnb:**
- https://www.searchlogistics.com/learn/statistics/airbnb-statistics/
- https://www.igms.com/airbnb-statistics/
- https://www.igms.com/airbnb-statistics/
- https://www.searchlogistics.com/learn/statistics/airbnb-statistics/


## Kenapa Bangkok?

Bangkok adalah ibu kota Thailand yang juga merupakan salah satu kota paling populer di dunia untuk pariwisata. Menurut Mastercard Global Destination Cities Index 2019, Bangkok menempati urutan pertama sebagai kota dengan kunjungan wisatawan internasional terbanyak di dunia dengan lebih dari 22 juta kunjungan wisatawan internasional yang menginap semalam. **(Sumber: https://www.mastercard.com/news/insights/2019/global-destination-cities-index-2019-1/)**

***Alasan kenapa banyak orang tertarik ke Bangkok antara lain:**
- Banyak destinasi budaya dan sejarah seperti Grand Palace, Wat Arun, dan Wat Pho **(sumber: https://www.klook.com/id/blog/tempat-wisata-di-bangkok/)**
- Kuliner jalanan terbaik di Asia (seperti di Khao San Road dan Chatuchak Market) **(Sumber: https://www.traveloka.com/id-id/explore/activities/rekomendasi-night-market-bangkok-ta/298903)**
- Surga belanja murah di area Pratunam, Siam, dan Asok **(Sumber: https://www.klook.com/id/blog/belanja-di-bangkok/)**
- Akses transportasi mudah (MRT, BTS), dan lokasi strategis untuk menjangkau Pattaya atau Chiang Mai **(Sumber: https://www.klook.com/id/blog/panduan-transportasi-bangkok/ & https://www.tempo.co/hiburan/menjajal-bts-skytrain-dan-mrt-bangkok-intip-kemudahannya-768697)**

Dengan besarnya minat wisatawan terhadap kota ini, kebutuhan akan akomodasi alternatif di luar hotel juga ikut meningkat. Di sinilah peran Airbnb menjadi penting sebagai solusi tempat tinggal yang lebih fleksibel dan sering kali lebih terjangkau dibanding hotel.

Banyak guest Airbnb di Bangkok yang memilih properti di area seperti:
- **Sukhumvit**: modern dan dekat pusat belanja
- **Khlong Toei**: dekat terminal dan pasar
- **Bang Rak**: kawasan sejarah dan budaya

**Referensi tambahan:**
- https://kumparan.com/redaksiportalmadura/7-alasan-mengapa-bangkok-disukai-oleh-banyak-turis-dari-seluruh-dunia-1536210598560749773
- https://trip101.com/id/artikel/10-airbnb-terbaik-di-sukhumvit-bangkok-thailand-id
- https://www.airbnb.co.id/bang-rak-thailand/stays
- https://www.airbnb.co.id/rooms/6164354
- https://www.airbnb.co.id/khlong-toei-thailand/stays/houses

Airbnb di Bangkok umumnya digunakan oleh wisatawan internasional yang ingin hemat biaya, tinggal lebih lama, atau sekadar menghindari keramaian hotel.

---

# DATA UNDERSTANDING

## **Tentang Dataset**

Dataset yang digunakan pada project ini adalah kumpulan **data listing Airbnb di Bangkok**, yaitu data properti yang dipublikasikan dan tersedia untuk disewa oleh tamu (guest) di platform Airbnb.
- [Link Google Drive Dataset (.csv)](https://drive.google.com/file/d/14ZAwaj9DmuxvI7DMOBeWbBXg0kTe95sE/view?usp=drive_link)
- [Link Data Dictionary (.pdf)](https://drive.google.com/file/d/1FCZkg_OPnN5C6jcy9-YpN-qnPy0ZP0Eq/view?usp=drive_link)

**Catatan penting:**
- Ini adalah **data listing**, bukan data transaksi aktual. Jadi, tidak terdapat data tentang jumlah pemesanan atau pendapatan, atau lama tinggal sesungguhnya.
- Artinya, kita hanya bisa menganalisis properti yang *terdaftar*, bukan yang *benar-benar disewa*.

**Berikut adalah penjelasan tiap kolom dalam dataset:**

| Kolom                          | Deskripsi                                                                 |
|--------------------------------|--------------------------------------------------------------------------|
| `id`                           | ID unik untuk setiap properti (listing)                                  |
| `name`                         | Nama atau judul listing                                                  |
| `host_id`                      | ID unik pemilik properti (host)                                          |
| `host_name`                    | Nama pemilik properti (host)                                            |
| `neighbourhood`               | Area atau distrik tempat listing berada (misalnya: Sukhumvit, Khlong Toei) |
| `latitude`                     | Koordinat geografis lintang properti                                     |
| `longitude`                    | Koordinat geografis bujur properti                                       |
| `room_type`                    | Jenis ruang yang ditawarkan: Entire home/apt, Private room, Shared room |
| `price`                        | Harga listing per malam dalam mata uang lokal                            |
| `minimum_nights`               | Minimum jumlah malam yang harus dipesan                                  |
| `number_of_reviews`            | Total jumlah ulasan dari tamu (guest)                                    |
| `last_review`                  | Tanggal terakhir ulasan ditulis                                          |
| `reviews_per_month`            | Rata-rata jumlah ulasan per bulan                                        |
| `calculated_host_listings_count` | Jumlah listing lain yang dimiliki oleh host tersebut                    |
| `availability_365`             | Total jumlah hari listing tersedia untuk disewa dalam setahun            |
| `number_of_reviews_ltm`        | Jumlah review dalam 12 bulan terakhir (Last Twelve Months)               |

## **Data Cleaning Summary**
### **Apa aja yang udah saya laukan di tahap data celaning**
1. **Drop Kolom Tidak Relevan**
   - `Unnamed: 0` dihapus karena hanya index hasil ekspor.

2. **Validasi Format**
   - `last_review` dikonversi ke format **datetime**

3. **Penanganan Missing Value**
   - `reviews_per_month`: Missing → diisi **0**
   - `last_review`: Missing → **dibiarkan NaT** karena penting untuk deteksi listing tidak aktif.
   - `host_name`: Missing → diisi `'Unknown'`
   - `name`: Missing (sangat sedikit) → baris dihapus

4. **Hapus Nilai Tidak Masuk Akal**
   - Listing dengan `price = 0` dihapus (**1 baris**)
   - `minimum_nights > 365` → **dipertahankan**, digunakan untuk segmentasi long-stay

5. **Normalisasi Data Kategorikal**
   - `neighbourhood`: kapitalisasi + perbaikan typo
   - Contoh: `'Yan Na Wa'` → `'Yan Nawa'`, `'Parthum Wan'` → `'Pathum Wan'`

6. **Cek & Validasi Duplikasi**
   - Tidak ditemukan **baris duplikat**
   - `host_id` boleh duplikat (karena 1 host bisa punya banyak listing)
   - Kombinasi `host_id` & `host_name` juga **konsisten**

7. **Deteksi Outlier (IQR & Boxplot)**
   - `price`: 1.402 outlier → **dipertahankan** untuk segmen premium
   - `minimum_nights`: 3.168 outlier → **long-stay**, **tidak dihapus**
   - `number_of_reviews`: 2.240 outlier → justru jadi indikator popularitas

---

### Hasil Akhir Data Cleaning

| Aspek                  | Hasil                                                                 |
|------------------------|-----------------------------------------------------------------------|
| Dimensi Akhir Dataset  | 15.845 baris × 16 kolom                                               |
| Missing Value          | Hanya `last_review` (36%) yang dibiarkan karena penting untuk analisis |
| Outlier                | Ditetapkan sebagai **bagian dari analisis**, tidak dihapus             |
| Format & Konsistensi   | Sudah distandarkan, semua kolom datetime, kategorikal, dan numerik valid |
| Siap Analisis?         | **Sudah 100% siap** untuk tahap EDA dan analisis popularitas listing |

**Data Sudah Siap untuk EDA dan Analisis:**
- Semua tahap preprocessing sudah selesai.
- Struktur data sudah bersih dan tidak mengandung noise besar.
- Tipe data sudah sesuai (datetime, float, int, object).

---

# Data Analysis

## Business Problem Utama
**Bagaimana karakteristik listing Airbnb yang aktif dan disukai wisatawan di Bangkok, serta bagaimana insight ini bisa membantu host dan platform dalam meningkatkan performa listing?**

---

## Konteks Bisnis
Airbnb merupakan platform yang mempertemukan host (pemilik properti) dengan guest (penyewa). Kesuksesan platform sangat bergantung pada keterlibatan tamu dan kualitas listing. Listing yang aktif dan sering mendapat review biasanya:
- Memiliki visibilitas tinggi di pencarian
- Menarik lebih banyak tamu
- Meningkatkan kepercayaan calon penyewa

Dengan demikian, memahami **faktor-faktor yang berkontribusi terhadap jumlah review tinggi (popularitas)** sangat penting bagi host dan tim manajemen Airbnb.

---

## Definisi Listing Populer
- Listing populer diukur dari **jumlah review total (number_of_reviews)**, sebagai indikator keterlibatan dan kepuasan tamu.
- `last_review` tetap digunakan untuk validasi waktu keterkinian, namun **tidak menjadi metrik utama** karena banyak listing aktif tidak mencantumkan tanggal ulasan terakhir.

---

## Struktur Analisis

### A. Analisis Utama =  
1. **Regresi Poisson untuk Menilai Fator-Faktor Penentu Popularitas**
   Tujuan Analisis:
   - Mengevaluasi pengaruh simultan dari berbagai faktor terhadap **popularitas listing** yang diukur melalui **jumlah review (number_of_reviews)**. Analisis ini dapat digunakan untuk:
   - Menilai kekuatan pengaruh tiap variabel seperti tipe kamar, harga, ketersediaan, dan minimum stay.
   - Menyusun strategi berbasis data untuk host dan platform.


2. **Korelasi Ketersediaan Listing dan Jumlah Review**
   - Variabel: `availability_365` vs `number_of_reviews`
   - Tujuan: Apakah listing yang selalu tersedia cenderung lebih banyak dipesan?

3. **Room Type vs Jumlah Review**
   - Variabel: `room_type` vs `number_of_reviews`
   - Tujuan: Tipe kamar mana yang paling disukai wisatawan?

4. **Minimum Nights vs Jumlah Review**
   - Variabel: `minimum_nights` vs `number_of_reviews`
   - Tujuan: Apakah minimum nights yang tinggi membatasi pemesanan?

5. **Harga Listing dan Jumlah Review**
   - Variabel: `price` vs `number_of_reviews`
   - Tujuan: Apakah harga listing memengaruhi minat dan popularitas?

6. **Segmentasi Listing Populer vs Tidak Populer**
   - Segmentasi berdasarkan Q1 dan Q3 dari `number_of_reviews`
   - Tujuan: Membedakan karakteristik listing populer dan tidak

7. **Performa Lokasi Berdasarkan Jumlah Review**
   - Variabel: `neighbourhood` vs `number_of_reviews`
   - Tujuan: Lokasi/distrik mana yang memiliki listing paling populer?

### B. Analisis Pendukung
8. **Distribusi Harga dan Kategorisasi**
   - Tujuan: Kelompokkan listing berdasarkan range harga

9. **Top 10 Neighbourhood berdasarkan Room Type**
   - Tujuan: Melihat distrik favorit berdasarkan jenis akomodasi

10. **Top 10 Neighbourhood Berdasarkan Harga Median**
   - Tujuan: Menentukan wilayah premium vs ekonomis

11. **Top 10 Host Berdasarkan Jumlah Review**
   - Tujuan: Melihat host yang paling menarik bagi tamu

12. **Distribusi Listing Berdasarkan Harga & Lokasi**
   - Tujuan: Apakah harga tinggi terkonsentrasi di lokasi tertentu?

13. **Scatterplot Harga vs Jumlah Review**
   - Tujuan: Apakah harga tinggi selalu berbanding lurus dengan popularitas?

14. **Analisis Tambahan : Pengaruh Penggunaan Kata Kunci dalam Nama Listing terhadap Popularitas Listing Airbnb Bangkok**
   - Tujuan: Menilai apakah penggunaan kata kunci tertentu dalam nama listing (seperti "BTS", "Pool", "Wifi", dll) berpengaruh terhadap **popularitas listing**, yang diukur dari **jumlah ulasan (number_of_reviews)**.
   
## Tujuan Akhir Proyek
- Memberikan **data-driven insights** bagi host dan manajemen Airbnb
- Memberikan rekomendasi berdasarkan data:
  - Harga optimal
  - Lokasi strategis
  - Jenis kamar disukai tamu
  - Minimum stay yang ideal

---

## Ringkasan Analisis yang Dilakukan

### Statistik Inferensial:
- **Regresi Poisson (GLM)**: Menilai pengaruh simultan variabel (room_type, price, availability_365, minimum_nights) terhadap jumlah review
- **Kruskal-Wallis Test**: Menguji beda jumlah review antar distrik (neighbourhood) dan tipe kamar
- **Spearman Correlation**: Hubungan antara price, availability_365, dan minimum_nights terhadap number_of_reviews

### Visualisasi & EDA:
- Scatterplot, Bar chart, Boxplot, Heatmap, Map Plot
- Kategorisasi harga (Low, Mid, High, Premium)
- Segmentasi listing populer vs tidak populer (berdasarkan Q1 & Q3 number_of_reviews)
- Distribusi spasial lokasi listing populer
- Analisis kata kunci dalam nama listing

---

## Insight dari Masing-Masing Analisis

### 1. Regresi Poisson (GLM)
Model ini menunjukkan bahwa semua variabel yang diuji (room_type, price, availability_365, dan minimum_nights) memiliki pengaruh signifikan terhadap jumlah ulasan. Listing dengan tipe Entire home memiliki probabilitas lebih tinggi untuk mendapatkan ulasan dibanding tipe lainnya. Kenaikan harga, penurunan ketersediaan, dan peningkatan minimum nights secara signifikan menurunkan jumlah review.
- **Rekomendasi:** Host sebaiknya menggunakan tipe Entire, menjaga harga tetap kompetitif, menetapkan minimum stay yang rendah, dan meningkatkan availability.

### 2. Korelasi Availability vs Number of Reviews
Terdapat korelasi positif yang bermakna antara ketersediaan listing dan jumlah ulasan. Semakin sering listing tersedia sepanjang tahun, semakin banyak review yang diterima.
- **Rekomendasi:** Aktifkan listing secara konsisten dan pastikan kalender ketersediaan diperbarui secara rutin agar lebih terlihat oleh calon tamu.

### 3. Room Type vs Review
Tipe kamar Entire home/apartment paling sering dipesan, disusul oleh private room dan shared room. Tipe shared room memiliki jumlah review paling rendah.
- **Rekomendasi:** Host baru disarankan menggunakan tipe Entire home untuk meningkatkan peluang dipesan dan memperoleh ulasan.

### 4. Minimum Nights vs Review
Listing dengan minimum stay yang tinggi memiliki jumlah ulasan lebih rendah. Korelasi negatif menunjukkan bahwa semakin panjang batas minimum menginap, semakin kecil kemungkinan listing dipesan dan diulas.
- **Rekomendasi:** Tetapkan minimum stay antara 1–3 malam untuk menarik berbagai jenis tamu, termasuk wisatawan jangka pendek.

### 5. Harga vs Review
Listing dengan harga mahal cenderung mendapat lebih sedikit review. Sebaliknya, listing dengan harga terjangkau mendapatkan review lebih banyak. Hal ini menunjukkan adanya sensitivitas harga di kalangan tamu Airbnb di Bangkok.
- **Rekomendasi:** Untuk host baru atau listing yang sepi, sebaiknya menetapkan harga awal yang kompetitif di bawah 2.500 Baht.

### 6. Segmentasi Listing Populer
Listing populer (≥ Q3 jumlah review) didominasi oleh Entire home, harga menengah ke bawah, dan minimum nights rendah. Sebaliknya, listing tidak populer cenderung memiliki kombinasi harga tinggi dan minimum stay tinggi.
- **Rekomendasi:** Host dapat mengadopsi strategi dari listing populer, seperti fleksibilitas durasi menginap dan penawaran harga yang kompetitif.

### 7. Performa Lokasi Berdasarkan Jumlah Review
Distrik seperti Khlong Toei, Watthana, dan Bang Rak menunjukkan performa tinggi dalam hal jumlah review. Hasil uji Kruskal-Wallis juga membuktikan bahwa perbedaan ini signifikan.
- **Rekomendasi:** Host sebaiknya memilih lokasi dengan volume wisatawan tinggi, akses transportasi mudah, atau kedekatan dengan landmark terkenal.

### 8. Distribusi Harga dan Kategorisasi
Sebagian besar listing berada dalam kisaran harga 900–2.429 Baht. Distribusi harga sangat skewed karena outlier seperti listing dengan harga di atas 100.000 Baht.
- **Rekomendasi:** Host dapat menggunakan segmentasi harga ini (Low–Mid–High–Premium) sebagai panduan strategi penetapan harga sesuai posisi listing.

### 9. Room Type per Distrik
Setiap distrik menunjukkan preferensi dominan terhadap tipe kamar tertentu. Misalnya, Watthana didominasi oleh Entire home, sedangkan Din Daeng lebih banyak memiliki Private room.
- **Rekomendasi:** Host disarankan melakukan riset pasar berdasarkan lokasi sebelum menetapkan tipe kamar yang akan ditawarkan.

### 10. Harga Median per Distrik
Wilayah premium seperti Watthana, Sathorn, dan Khlong San memiliki harga median lebih tinggi. Namun, tidak selalu berkorelasi dengan jumlah review yang tinggi.
- **Rekomendasi:** Host harus realistis dalam menetapkan harga sesuai ekspektasi pasar lokal, tidak semua distrik cocok untuk premium listing.

### 11. Top 10 Host Berdasarkan Review
Beberapa host dengan nama seperti Evan dan Tony memiliki review tertinggi secara total. Kemungkinan mereka menggunakan strategi SEO, listing ganda, dan harga bersaing.
- **Rekomendasi:** Host lain dapat belajar dari strategi visual, keyword, dan promosi yang digunakan oleh power host ini.

### 12. Heatmap Distribusi Harga vs Lokasi
Listing dengan kategori harga Premium banyak terkonsentrasi di distrik seperti Sathorn, Watthana, dan Bang Rak. Sementara distrik seperti Din Daeng lebih didominasi harga Low hingga Mid.
- **Rekomendasi:** Sesuaikan positioning harga dengan daya beli dan ekspektasi tamu di wilayah tertentu.

### 13. Scatterplot Harga vs Jumlah Review
Terdapat pola yang menunjukkan bahwa harga tinggi tidak menjamin banyak review. Banyak listing murah justru memiliki review lebih banyak dan stabil.
- **Rekomendasi:** Fokus pada value for money dan review positif daripada menaikkan harga tanpa diferensiasi layanan.

### 14. Pengaruh Kata Kunci dalam Nama Listing
Kata-kata seperti "BTS", "Wifi", "Pool", dan "Central" lebih sering digunakan dalam listing populer. Artinya, SEO dan first impression listing memainkan peran penting.
- **Rekomendasi:** Gunakan nama listing yang mengandung kata kunci relevan agar lebih mudah ditemukan dan menarik perhatian tamu.

---

## Insight Keseluruhan
Berdasarkan seluruh rangkaian analisis, dapat disimpulkan bahwa listing Airbnb yang paling populer di Bangkok menunjukkan karakteristik sebagai berikut:
- Menggunakan **Entire home/apartment** sebagai room type
- Memiliki **harga kompetitif**, umumnya antara **900–2.500 Baht**
- Menetapkan **minimum stay fleksibel** (1–2 malam)
- Memiliki **availability tinggi** (aktif sepanjang tahun)
- Berlokasi di **distrik wisata utama** seperti Khlong Toei, Watthana, dan Sathorn
- Menggunakan **kata kunci strategis** pada nama listing ("Wifi", "BTS", "Central")

Strategi kombinasi dari elemen-elemen ini meningkatkan peluang listing untuk lebih sering muncul di hasil pencarian, dipesan, dan mendapatkan review positif.


---

## Actionable Recommendations

### Untuk Host Baru
- Buat listing bertipe **Entire home/apt** agar menarik pasar luas.
- Fokus listing di area dengan traffic tinggi seperti **Khlong Toei**, **Watthana**, atau **Sathorn**.
- Tetapkan harga kompetitif (antara **900–2.500 Baht**), terutama untuk listing baru.
- Minimalkan **minimum stay** menjadi 1–2 malam agar lebih fleksibel.
- Tambahkan kata kunci penting di nama listing seperti "Near BTS", "Pool", "Central", dan "Wifi" untuk memaksimalkan visibilitas.

### Untuk Host Eksisting
- Evaluasi ulang harga listing jika sepi review dan sesuaikan dengan kategori harga wilayah.
- **Perbarui kalender secara berkala** untuk menjaga listing tetap aktif.
- Pertimbangkan **optimalisasi keyword** untuk meningkatkan Click-Through Rate (CTR).
- Bandingkan listing dengan power host dan pelajari apa yang membedakan mereka (foto, deskripsi, fasilitas, dan harga).

### Untuk Tim Manajemen Airbnb
- Optimalkan algoritma pencarian untuk memprioritaskan listing yang sesuai dengan pola sukses di atas.
- Kembangkan sistem **rekomendasi otomatis** kepada host berdasarkan performa historis data.
- Sediakan panduan strategi harga dan keyword berdasarkan data tiap distrik agar membantu host baru.
- Dorong host agar melakukan perbandingan harga dan keyword dengan power host di sekitarnya.

---



