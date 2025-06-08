# 💬 Sentiment Analysis Project: Text Classification on User Reviews

## 📌 Deskripsi
Proyek ini adalah implementasi machine learning sederhana untuk mengklasifikasikan sentimen dari teks review aplikasi ke dalam tiga kategori: **positif**, **netral**, dan **negatif**. Model yang digunakan:

- **SVM + TF-IDF**
- **Random Forest + TF-IDF**
- **Random Forest + CountVectorizer**

Dataset dikumpulkan secara otomatis melalui **web scraping review aplikasi ChatGPT dari Google Play Store** menggunakan Python.

Model-model ini dilatih menggunakan dataset teks berbahasa Indonesia, lalu disimpan menggunakan `joblib` dan digunakan kembali untuk prediksi pada teks baru.

---

## 🧠 Teknologi & Library
- Python 
- Scikit-learn
- Pandas
- Numpy
- Joblib

---

## 📂 Struktur File
```
├── 📁 Models/                      # Berisi file model (*.pkl)
├── Analisis_Sentimen_ChatGpt.ipynb # Notebook training dan evaluasi model
├── Inference.ipynb                 # Notebook untuk prediksi review baru
├── Review_scraping.ipynb           # Notebook untuk scraping review dari Play Store
├── ulasan_chatgpt.csv              # Dataset hasil scraping
└── requirements.txt                # File dependency
```

## 🔍 Contoh Output Prediksi
```
Hasil Prediksi Sentimen:
Kalimat: Aplikasi ini sering error dan sering memberikan jawaban yang salah
SVM + TF-IDF     → negative
RF + TF-IDF      → negative
RF + CountVector → negative
--------------------------------------------------
Kalimat: Bagus sekali aplikasinya, sangat membantu
SVM + TF-IDF     → positive
RF + TF-IDF      → positive
RF + CountVector → positive
--------------------------------------------------
Kalimat: ChatGPT cukup baik, meskipun ada beberapa jawaban yang kurang tepat.
SVM + TF-IDF     → neutral
RF + TF-IDF      → neutral
RF + CountVector → neutral
--------------------------------------------------
```
