# Big Data Project — Kelompok 4

## Analisis Pengelompokan Opini Publik terhadap Pemerintahan Prabowo–Gibran pada Komentar YouTube Menggunakan Algoritma K-Means Clustering

## 1. Deskripsi Proyek

Proyek ini merupakan bagian dari tugas mata kuliah **Big Data** yang bertujuan untuk menganalisis dan mengelompokkan opini publik mengenai pemerintahan Prabowo–Gibran berdasarkan komentar pengguna YouTube.

Penelitian ini menggunakan pendekatan *Text Mining* dan *Natural Language Processing* (NLP) untuk mengolah data teks dari komentar YouTube. Data yang telah dikumpulkan akan melalui beberapa tahapan, mulai dari pengumpulan data, pembersihan teks, preprocessing, pembobotan kata menggunakan TF-IDF, hingga pengelompokan menggunakan algoritma K-Means Clustering.

Hasil pengelompokan akan dianalisis untuk mengetahui tema atau pola pembahasan yang muncul dalam komentar publik.

**Penelitian ini berfokus pada pengelompokan opini (clustering), bukan analisis sentimen.** Dengan demikian, sistem tidak secara langsung menentukan apakah suatu komentar bersifat positif, negatif, atau netral.

## 2. Tujuan Proyek

Tujuan dari proyek ini adalah:

1. Mengumpulkan data komentar YouTube yang berkaitan dengan pemerintahan Prabowo–Gibran.
2. Melakukan pembersihan dan preprocessing terhadap data teks agar siap digunakan dalam proses analisis.
3. Mengubah data teks menjadi representasi numerik menggunakan metode TF-IDF.
4. Mengelompokkan komentar berdasarkan kemiripan karakteristik teks menggunakan algoritma K-Means Clustering.
5. Mengidentifikasi dan menginterpretasikan tema pembahasan yang terbentuk dari setiap cluster.
6. Menyajikan hasil analisis dalam bentuk visualisasi dan laporan yang mudah dipahami.

## 3. Metodologi

Proyek ini menggunakan beberapa metode dan tahapan pengolahan data sebagai berikut:

| Tahapan | Metode / Teknik | Keterangan |
|---|---|---|
| Data Collection | YouTube Data API v3 | Mengumpulkan komentar dari video YouTube yang relevan. |
| Data Cleaning | Text Cleaning | Menghapus data kosong, duplikat, spam, dan karakter yang tidak diperlukan. |
| Text Preprocessing | Tokenization, Stopword Removal, Stemming | Membersihkan dan mempersiapkan teks untuk proses analisis. |
| Feature Extraction | TF-IDF | Mengubah teks menjadi representasi numerik berdasarkan bobot kata. |
| Clustering | K-Means Clustering | Mengelompokkan komentar berdasarkan kemiripan representasi teks. |
| Evaluation | Elbow Method dan Silhouette Score | Membantu menentukan dan mengevaluasi jumlah cluster. |
| Interpretation | Cluster Analysis | Mengidentifikasi karakteristik dan tema dari setiap kelompok komentar. |

## 4. Alur Pengerjaan

Secara keseluruhan, proses pengerjaan proyek dibagi menjadi 11 tahapan:

1. **Literature Review** — Mempelajari penelitian terdahulu dan teori yang relevan.
2. **Data Collection** — Mengumpulkan komentar YouTube menggunakan YouTube Data API v3.
3. **Exploratory Data Analysis (EDA)** — Memahami karakteristik awal dataset.
4. **Data Cleaning** — Membersihkan data dari komentar kosong, duplikat, dan data tidak relevan.
5. **Text Preprocessing** — Melakukan normalisasi, tokenisasi, stopword removal, dan stemming.
6. **Feature Extraction** — Mengubah data teks menjadi matriks numerik menggunakan TF-IDF.
7. **Model Development** — Menerapkan algoritma K-Means Clustering.
8. **Model Evaluation** — Mengevaluasi hasil clustering menggunakan Elbow Method dan Silhouette Score.
9. **Cluster Interpretation** — Mengidentifikasi tema dan karakteristik setiap cluster.
10. **Data Visualization** — Menampilkan hasil analisis melalui grafik dan visualisasi.
11. **Reporting** — Menyusun hasil penelitian, kesimpulan, dan dokumentasi proyek.

## 5. Teknologi dan Tools

Teknologi yang digunakan dalam proyek ini meliputi:

- **Python** — Bahasa pemrograman utama untuk pengolahan dan analisis data.
- **Google Colab** — Lingkungan pengembangan untuk menjalankan kode Python.
- **YouTube Data API v3** — API untuk mengumpulkan data komentar YouTube.
- **Pandas** — Pengolahan dan manipulasi dataset.
- **NumPy** — Operasi komputasi numerik.
- **NLTK** — Pendukung proses pengolahan teks.
- **Sastrawi** — Stemming bahasa Indonesia.
- **Scikit-learn** — TF-IDF, K-Means, dan evaluasi clustering.
- **Matplotlib dan Seaborn** — Visualisasi hasil analisis.
- **WordCloud** — Visualisasi kata-kata yang sering muncul.

## 6. Struktur Repository

```text
Big-Data-Project-Kelompok-4/
│
├── README.md
│
├── notebooks/
│   └── big_data_analysis.ipynb
│
├── data/
│   ├── raw/
│   │   └── .gitkeep
│   │
│   ├── processed/
│   │   └── .gitkeep
│   │
│   └── results/
│       └── .gitkeep
│
├── outputs/
│   ├── visualizations/
│   │   └── .gitkeep
│   │
│   └── reports/
│       └── .gitkeep
│
└── requirements.txt
```

**Keterangan folder:**

- `notebooks/` — Menyimpan notebook Google Colab atau Jupyter Notebook.
- `data/raw/` — Menyimpan dataset mentah hasil pengumpulan komentar YouTube.
- `data/processed/` — Menyimpan dataset yang telah melalui proses cleaning dan preprocessing.
- `data/results/` — Menyimpan hasil pemodelan dan label cluster.
- `outputs/visualizations/` — Menyimpan grafik, Word Cloud, dan visualisasi lainnya.
- `outputs/reports/` — Menyimpan laporan dan dokumentasi hasil penelitian.
- `requirements.txt` — Daftar library Python yang dibutuhkan.

## 7. Pembagian Tugas Kelompok

Proyek ini dikerjakan oleh enam anggota dengan pembagian tanggung jawab sebagai berikut:

| Anggota | Tanggung Jawab |
|---|---|
| P1 | Research & Literature Review — Studi literatur, latar belakang, metodologi, dan penulisan laporan. |
| P2 | Data Collection — Pengumpulan data komentar YouTube dan dokumentasi sumber data. |
| P3 | Data Cleaning & Preprocessing — Pembersihan dataset dan pengolahan teks. |
| P4 | Machine Learning Development — Ekstraksi fitur TF-IDF dan implementasi K-Means. |
| P5 | Evaluation & Cluster Analysis — Evaluasi model dan interpretasi hasil clustering. |
| P6 | Visualization & Documentation — Visualisasi data, dokumentasi, dan penyusunan presentasi. |

## 8. Dataset

Data penelitian bersumber dari komentar publik pada video YouTube yang relevan dengan topik pemerintahan Prabowo–Gibran.

Pengumpulan data dilakukan menggunakan YouTube Data API v3 dengan mempertimbangkan relevansi video dan komentar terhadap topik penelitian.

Beberapa atribut data yang digunakan meliputi:

- `comment_id` — Identitas komentar.
- `video_id` — Identitas video sumber.
- `video_title` — Judul video.
- `comment` — Isi komentar.
- `published_at` — Waktu publikasi komentar.
- `like_count` — Jumlah suka pada komentar.

**Catatan:** Jumlah data akhir akan disesuaikan dengan hasil pengumpulan dan proses seleksi data. Dataset yang digunakan dalam analisis akan didokumentasikan sesuai tahapan pengolahannya.

## 9. Evaluasi dan Hasil yang Diharapkan

Evaluasi clustering dilakukan menggunakan:

1. **Elbow Method:** Membantu mengidentifikasi jumlah cluster yang sesuai berdasarkan perubahan nilai inertia.
2. **Silhouette Score:** Mengukur seberapa baik suatu data berada dalam cluster dibandingkan dengan cluster lainnya.

Setelah proses clustering selesai, setiap kelompok akan dianalisis berdasarkan kata-kata dominan, jumlah komentar, dan contoh komentar yang representatif.

Hasil akhirnya diharapkan dapat memberikan gambaran mengenai pola dan tema pembahasan yang muncul dalam komentar YouTube terkait pemerintahan Prabowo–Gibran.

## 10. Batasan Penelitian

Untuk menjaga ruang lingkup penelitian, terdapat beberapa batasan:

1. Data penelitian berasal dari komentar publik YouTube yang berhasil dikumpulkan melalui API.
2. Analisis dibatasi pada komentar yang relevan dengan topik pemerintahan Prabowo–Gibran.
3. Pengelompokan dilakukan berdasarkan kemiripan karakteristik teks, bukan berdasarkan label sentimen.
4. Hasil clustering bergantung pada kualitas data, proses preprocessing, dan konfigurasi model.
5. Hasil penelitian tidak dapat dianggap mewakili seluruh opini masyarakat Indonesia karena data berasal dari sumber dan komentar yang berhasil dikumpulkan.

## 11. Tim Pengembang

**Kelompok 4 — Mata Kuliah Big Data**

- P1 — Research & Literature Review
- P2 — Data Collection
- P3 — Data Cleaning & Preprocessing
- P4 — Machine Learning Development
- P5 — Evaluation & Cluster Analysis
- P6 — Visualization & Documentation

## 12. Status Proyek

**Status:** In Progress

Proyek ini dikembangkan secara kolaboratif sebagai pemenuhan tugas mata kuliah Big Data. Seluruh tahapan pengolahan data, implementasi model, evaluasi, dan dokumentasi akan diperbarui seiring perkembangan pengerjaan proyek.

---

*Big Data Project — Kelompok 4*  
*Universitas Hasanuddin*
