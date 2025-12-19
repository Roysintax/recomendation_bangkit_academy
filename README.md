# 📚 ABA-I Story Recommendation System

> **Bangkit Academy 2024 Capstone Project**
>
> API Sistem Rekomendasi Cerita Rakyat Indonesia berbasis *Content-Based Filtering* menggunakan Deep Learning.

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python)
![Flask](https://img.shields.io/badge/Flask-2.0-green?style=for-the-badge&logo=flask)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0-orange?style=for-the-badge&logo=tensorflow)
![MySQL](https://img.shields.io/badge/MySQL-Database-blue?style=for-the-badge&logo=mysql)

## 📖 Tentang Proyek

Proyek ini adalah bagian dari Capstone Project **ABA-I (Ayo Baca Indonesia)**. Sistem ini menyediakan API untuk merekomendasikan cerita atau buku berdasarkan kemiripan konten (Content-Based Filtering).

Model ini menganalisis fitur cerita seperti **Ringkasan (Overview)**, **Penulis**, **Asal Daerah**, dan **Genre** untuk memberikan saran bacaan yang relevan kepada pengguna.

## 🚀 Fitur Utama

* **Smart Recommendation:** Menggunakan TF-IDF dan Neural Network (TensorFlow/Keras) untuk menghitung kemiripan cerita.
* **RESTful API:** Endpoint sederhana untuk meminta rekomendasi cerita.
* **Database Integration:** Terhubung langsung dengan database MySQL untuk mengambil data cerita terbaru.
* **Text Preprocessing:** Pembersihan teks otomatis (Stopwords removal, Tokenization) khusus Bahasa Indonesia.

## 🛠️ Teknologi yang Digunakan

* **Backend Framework:** Flask
* **Machine Learning:** TensorFlow, Scikit-learn, NLTK, Pandas, NumPy
* **Database:** MySQL (via SQLAlchemy)
* **Server:** XAMPP (Local Development)

## 📂 Struktur Proyek

```text
.
├── app.py                  # Main Flask Application
├── book_recommendation.ipynb # Jupyter Notebook untuk Training Model
├── requirements.txt        # Daftar dependensi Python
├── data/
│   ├── storyy.csv          # Dataset mentah (CSV)
│   └── story_db.sql        # File dump database MySQL
├── model/
│   ├── rekomendasiByStoryID.h5  # Model Deep Learning yang sudah dilatih
│   └── vectorizer.pkl           # TF-IDF Vectorizer yang sudah disimpan
└── README.md               # Dokumentasi Proyek
