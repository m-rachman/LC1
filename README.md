[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/P4NZZEkH)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11411477&assignment_repo_type=AssignmentRepo)
# Live Code 1 - Set 3

---

## Assignment Objectives

*Live Code 1* ini dibuat guna mengevaluasi konsep Regression sebagai berikut:

- Mampu memahami konsep regression dengan Linear Regression.

- Mampu mempersiapkan data untuk digunakan dalam model Linear Regression.

- Mampu mengimplementasikan Linear Regression untuk membuat prediksi.

---

## Dataset Desciription

Description : anda adalah Data Scientist disebuah perusahaan Garment. Industri Pakaian adalah salah satu contoh kunci dari globalisasi industri era modern ini. Ini adalah industri yang sangat padat karya dengan banyak proses manual. Memenuhi permintaan global yang besar untuk produk pakaian sebagian besar bergantung pada kinerja produksi dan pengiriman karyawan di perusahaan manufaktur pakaian. Oleh karena itu, sangat diinginkan bagi para pengambil keputusan di industri pakaian untuk melacak, menganalisis, dan memprediksi kinerja produktivitas tim kerja di pabrik mereka.

| Column | Description |
| --- | --- |
| 01 date | Date in MM-DD-YYYY |
| 02 day | Day of the Week |
| 03 quarter | A portion of the month. A month was divided into four quarters |
| 04 department | Associated department with the instance |
| 05 team_no | Associated team number with the instance |
| 06 no_of_workers | Number of workers in each team |
| 07 no_of_style_change | Number of changes in the style of a particular product |
| 08 targeted_productivity | Targeted productivity set by the Authority for each team for each day |
| 09 smv | Standard Minute Value, it is the allocated time for a task |
| 10 wip | Work in progress. Includes the number of unfinished items for products |
| 11 over_time | Represents the amount of overtime by each team in minutes |
| 12 incentive | Represents the amount of financial incentive (in BDT) that enables or motivates a particular course of action |
| 13 idle_time | The amount of time when the production was interrupted due to several reasons |
| 14 idle_men | The number of workers who were idle due to production interruption |
| 15 actual_productivity | The actual % of productivity that was delivered by the workers. It ranges from 0-1 |


---

## Problems

Buatlah model Linear Regression untuk memprediksi **`actual_productivity`** karyawan menggunakan dataset yang disediakan. Dataset terlampir pada repository dan jawablah pertanyaan dibawah ini.

***Note : Anda diwajibkan untuk menjawab pertanyaan-pertanyaan dibawah ini. Namun, Anda juga dipersilakan untuk melakukan Exploratory Data Analysis (EDA) dan analisa model lainnya pada bagian Model Evaluation diluar pertanyaan yang diminta.***

### Lakukan pada bagian Exploratory Data Analysis (EDA)
1. Top level management meminta anda untuk melihat berapa persentase `actual_productivity` di dalam dataset yang melebihi atau sama dengan `targeted_productivity`. Buatkan visualisasinya kedalam pie chart, berikan analisa anda sebab top level management ingin melihat apakah target yang sudah di rencanakan sebelumnya masuk akal dan berjalan dengan baik. 

2. Top level management meminta anda untuk memberikan data rata-rata waktu `over_time` setiap bulan, rata-rata `actual_productivity` setiap bulan dan rata-rata `targeted_productivity` setiap bulan untuk menjawab pertanyaan sebagai berikut :
   a) bulan apa rata-rata waktu `over_time` paling tinggi?
   
   b) apabila waktu rata-rata `over_time` di konversi menjadi hari, berapa hari `over_time` di bulan pertama, kedua dan ketiga?

   c) berikan analisa anda apakah `over_time` yang diberikan perusahaan mampu menaikan `actual_productivity` dengan signifikan?

---

## Instruction

*Live Code 1* dikerjakan dalam format ***notebook (.ipynb)*** dengan beberapa **kriteria wajib** dibawah ini:

1. Machine learning framework yang digunakan adalah *Scikit-Learn*.

2. Ada penggunaan library visualisasi, seperti *matplotlib*, *seaborn*, atau yang lain.

3. Isi *notebook* harus mengikuti *outline* di bawah ini:
   1. Perkenalan
      > Bab pengenalan harus diisi dengan identitas, gambaran besar dataset yang digunakan, dan *objective* yang ingin dicapai.
   
   2. Import Libraries
      > *Cell* pertama pada *notebook* **harus berisi dan hanya berisi** semua *library* yang digunakan dalam *project*.

   3. Data Loading
      > Bagian ini berisi proses penyiapan data sebelum dilakukan eksplorasi data lebih lanjut. Proses Data Loading dapat berupa memberi nama baru untuk setiap kolom, mengecek ukuran dataset, dll.
   
   4. Exploratory Data Analysis (EDA)
      > Bagian ini berisi eksplorasi data pada dataset diatas dengan menggunakan query, grouping, visualisasi sederhana, dan lain sebagainya.
   
   5. Feature Engineering
      > Bagian ini berisi proses penyiapan data untuk proses pelatihan model, seperti pembagian data menjadi train-test, transformasi data (normalisasi, encoding, dll.), dan proses-proses lain yang dibutuhkan.

   6. Model Definition
      > Bagian ini berisi cell untuk mendefinisikan model. Jelaskan alasan menggunakan suatu algoritma/model, hyperparameter yang dipakai, jenis penggunaan metrics yang dipakai, dan hal lain yang terkait dengan model.

   7. Model Training
      > Cell pada bagian ini hanya berisi code untuk melatih model dan output yang dihasilkan. Lakukan beberapa kali proses training dengan hyperparameter yang berbeda untuk melihat hasil yang didapatkan. Analisis dan narasikan hasil ini pada bagian Model Evaluation.
   
   8. Model Evaluation
      > Pada bagian ini, dilakukan evaluasi model yang harus menunjukkan bagaimana performa model berdasarkan metrics yang dipilih. Hal ini harus dibuktikan dengan visualisasi tren performa dan/atau tingkat kesalahan model. **Lakukan analisis terkait dengan hasil pada model dan tuliskan hasil analisisnya**.

   9. Model Saving
      > Pada bagian ini, dilakukan proses penyimpanan model dan file-file lain yang terkait dengan hasil proses pembuatan model.

   10. Model Inference
       > Model yang sudah dilatih akan dicoba pada data yang bukan termasuk ke dalam train-set ataupun test-set. Data ini harus dalam format yang asli, bukan data yang sudah di-scaled.
   
   11. Pengambilan Kesimpulan
       > Pada bagian terakhir ini, **harus berisi** kesimpulan yang mencerminkan hasil yang didapat dengan *objective* yang sudah ditulis di bagian pengenalan.
    
4. *Notebook* harus diupload dalam akun GitHub masing-masing student untuk selanjutnya dinilai.

---

## Assignment Submission

- Simpan assignment pada sesi ini dengan nama `h8dsft_P1LC1_Set_3_<nama-students>.ipynb` misal `h8dsft_P1LC1_Set_3_raka_ardhi.ipynb`.

- Push Assigment yang telah Anda buat ke akun Github Classroom Anda masing-masing.

---

## Assignment Rubrics

### Code Review

| Criteria| Meet Expectations | Points |
| --- | --- | --- |
| Feature Engineering | Mampu melakukan preprocessing dataset sebelum melakukan proses modeling (split data, normalisasi, encoding, dll) | 35 pts |
| Linear Regression | Mengimplementasikan Linear Regression dan menentukan hyperparameter yang tepat dengan Scikit-Learn | 10 pts |
| Model Inference | Mencoba model yang telah dibuat dengan data baru | 10 pts |
| Runs Perfectly | Kode berjalan tanpa ada error. Seluruh kode berfungsi dan dibuat dengan benar | 10 pts |

### Readability

| Criteria | Meet Expectations | Points |
| --- | --- | --- |
| Tertata dengan Baik| Semua baris kode terdokumentasi dengan baik dengan Markdown untuk penjelasan kode | 15 pts |

```
Kriteria tertata dengan baik diantaranya adalah: 

1. Terdapat section Perkenalan yang jelas dan lengkap terkait masalah dan latar belakang masalah yang akan diselesaikan.
2. Tidak menyalin markdown dari tugas lain.
3. Import library rapih (terdapat dalam 1 cell dan tidak ada unused libs).
4. Pemakaian fungsi markdown yang optimal (Heading, text formating, dll).
5. Terdapat komentar pada setiap baris kode.
6. Adanya pemisah yang jelas antar section, dll.
7. Tidak adanya typo.
```

### Analysis

| Criteria | Meet Expectations | Points |
| --- | --- | --- |
| Model Analysis | Menganalisa informasi dari model yang telah dibuat | 35 pts |
| Overall Analysis | Menarik informasi/kesimpulan dari keseluruhan kegiatan yang dilakukan | 20 pts |

```
Contoh kriteria analisa yang baik diantaranya adalah: 

1. Terdapat penjelasan macam-macam hasil metric evaluasi dan interpretasinya terhadap kasus yang diselesaikan.
2. Dapat menjelaskan KELEBIHAN dan KELEMAHAN dari model yang dibuat DENGAN KAITANNYA DENGAN DOMAIN BUSINESS YANG DIHADAPI yang dibuktikan dengan eksplorasi sederhana (grafik, plot, teori, dll).
3. Dapat memberikan statement untuk improvement selanjutnya dari model yang dibuat. 
4. Dapat menyebutkan insight yang dapat diambil setelah proses EDA, dll.
```

---

```
Total Points : 135
```

---
## Notes

* **Deadline : pukul 12:15 WIB.**

* **Keterlambatan pengumpulan tugas mengakibatkan skor LC 1 menjadi 0.**
