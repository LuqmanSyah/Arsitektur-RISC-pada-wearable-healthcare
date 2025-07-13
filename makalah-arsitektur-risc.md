# Makalah
## Studi Kasus: Pemilihan Arsitektur Prosesor RISC untuk Perangkat Wearable Healthcare

---

### Daftar Anggota Kelompok

1. Luqman Syah  
2. [Silakan tambahkan nama anggota kelompok lain di sini]

---

### 1. Pendahuluan

Perkembangan teknologi wearable healthcare semakin pesat, ditandai dengan banyaknya perangkat seperti smartwatch, fitness tracker, dan alat monitoring kesehatan yang beredar di pasaran. Salah satu aspek paling krusial dalam pengembangan perangkat tersebut adalah pemilihan arsitektur prosesor. Arsitektur yang dipilih sangat mempengaruhi efisiensi daya, performa, serta biaya produksi perangkat.

Makalah ini membahas studi kasus pemilihan arsitektur prosesor **RISC (Reduced Instruction Set Computer)** untuk perangkat wearable healthcare, serta membandingkannya dengan arsitektur lain seperti **CISC (Complex Instruction Set Computer)**. Selain itu, makalah ini juga mengulas tren industri dan contoh nyata implementasi arsitektur RISC.

---

### 2. Konsep Dasar Arsitektur Prosesor

**RISC (Reduced Instruction Set Computer)** adalah arsitektur prosesor yang menggunakan kumpulan instruksi sederhana dan seragam. Setiap instruksi biasanya dapat dieksekusi dalam satu siklus clock, sehingga pipeline dapat dioptimalkan dengan mudah. Sebaliknya, **CISC (Complex Instruction Set Computer)** menggunakan instruksi yang lebih kompleks dan bervariasi, sehingga pipeline menjadi lebih rumit.

| RISC                  | CISC                    |
|-----------------------|-------------------------|
| Instruksi sederhana   | Instruksi kompleks      |
| Pipeline optimal      | Pipeline lebih rumit    |
| Hemat daya            | Konsumsi daya lebih tinggi |
| Contoh: ARM, RISC-V   | Contoh: x86 (Intel/AMD) |

---

### 3. Keunggulan RISC untuk Wearable Healthcare

#### 3.1 Efisiensi Daya  
Arsitektur RISC sangat hemat daya karena instruksinya sederhana dan pipeline mudah dioptimalkan. Hal ini penting untuk perangkat wearable yang bergantung pada baterai.

#### 3.2 Kinerja Tinggi  
Pipeline pada prosesor RISC dapat berjalan sangat efisien, sehingga pemrosesan data sensor dan komunikasi dapat dilakukan dengan cepat.

#### 3.3 Desain Hardware Sederhana dan Murah  
Chip berbasis RISC biasanya berukuran kecil dan murah diproduksi, sehingga cocok untuk perangkat wearable yang berorientasi pada produksi massal.

#### 3.4 Dukungan Ekosistem  
Arsitektur RISC, khususnya ARM, telah menjadi standar industri untuk perangkat wearable dan mobile. Dukungan software, tools, dan developer sangat luas.

---

### 4. Pipeline dan Compiler pada RISC

#### 4.1 Pipeline Instruksi  
Instruksi seragam pada RISC memudahkan pembagian pipeline menjadi tahapan tetap seperti Fetch, Decode, Execute, Memory, dan Write-back. Pipeline minim hambatan (hazard) dan mudah dioptimalkan.

#### 4.2 Peran Compiler  
Compiler pada RISC berperan penting dalam mengatur urutan instruksi (instruction scheduling) agar pipeline berjalan efisien dan menghindari stall akibat hazard.

---

### 5. Hazard Pipeline pada RISC

- **Data Hazard:** Lebih mudah diatasi karena instruksi seragam dan sederhana.
- **Control Hazard:** Branch prediction dan delay slot lebih mudah diterapkan pada RISC.
- **Structural Hazard:** Desain hardware yang sederhana membuat hazard jenis ini lebih mudah diprediksi dan dihindari.

---

### 6. Tren Industri dan Implementasi Nyata

#### 6.1 Dominasi ARM (RISC)
ARM merupakan arsitektur RISC yang mendominasi pasar smartphone, wearable, dan embedded systems karena efisiensi daya dan performa tinggi.  
**Contoh:**  
- Smartphone: Snapdragon (Qualcomm), Exynos (Samsung), Apple A-series (iPhone)  
- Wearable: Apple Watch, Samsung Galaxy Watch, Huawei Watch, Xiaomi Mi Band  
- IoT: Raspberry Pi, Arduino (modern), ESP32

#### 6.2 Perkembangan RISC-V
RISC-V adalah arsitektur RISC open-source yang mulai banyak digunakan di industri, misalnya oleh Western Digital untuk controller SSD, SiFive untuk chip IoT, dan beberapa perangkat AI edge (Kendryte K210).

---

### 7. Rekomendasi

Berdasarkan analisis di atas, arsitektur RISC (misal: ARM, RISC-V) **sangat direkomendasikan** untuk perangkat wearable healthcare karena:

- Efisiensi daya yang sangat baik
- Pipeline instruksi yang optimal
- Desain hardware sederhana dan biaya rendah
- Dukungan ekosistem dan industri yang luas
- Sudah terbukti di banyak produk wearable terkemuka

---

### 8. Kesimpulan

Pemilihan arsitektur prosesor sangat menentukan keberhasilan perangkat wearable healthcare. RISC menjadi pilihan utama karena efisiensi daya, performa, dan dukungan ekosistem yang luas. Penggunaan ARM dan RISC-V telah terbukti secara nyata dalam produk-produk wearable dan embedded di industri.

---

### 9. Referensi

1. ARM Holdings. “ARM Architecture Reference Manual”.  
2. RISC-V Foundation. “RISC-V Overview”.  
3. Qualcomm, Samsung, Apple, MediaTek – Official websites and product documentation.  
4. Western Digital, SiFive – RISC-V adoption news.  
5. Sumber lain terkait pipeline, compiler, dan hazard pada arsitektur prosesor.
