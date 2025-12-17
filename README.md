#📝 Project Overview

Proyek ini bertujuan untuk menganalisis teks forum berbahasa Indonesia dan mengelompokkannya ke tiga jenis:
- Sentimen → positif, negatif, atau netral
- Emosi → marah, senang, sedih, takut, atau cinta
- Toxicity → apakah komentar bersifat toxic atau aman
Proyek ini fokus pada moderasi konten dan memahami opini pengguna secara otomatis, tanpa perlu cek manual satu per satu.

##🔧 What We Built
- Data dibersihkan dari noise (URL, angka, huruf random, dsb)
- Stopwords dihapus dan kata distemming memakai Sastrawi
- Teks dikonversi menjadi angka dengan TF-IDF (5.000 fitur)
- Kami uji dua model:
  - Naive Bayes
  - Support Vector Machine
- Lalu dilakukan hyperparameter tuning untuk performa terbaik

##🚀 Key Results
SVM memberi hasil paling stabil dan unggul dibanding Naive Bayes.
Pencapaian akurasi terbaik:
- Toxicity: ~88%
- Sentiment: ~70%
- Emotion: ~62%
Toxicity menjadi task paling kuat karena pola bahasanya lebih eksplisit.

##💡 Why This Matters
Proyek ini cocok untuk:
- Moderasi komentar otomatis
- Mendeteksi ujaran kebencian
- Membaca tren opini publik
- Analisis sosial berbasis teks Indonesia

##🛠 Tech Stack
- Python (Scikit-learn)
- TF-IDF Vectorizer
- SVM & Naive Bayes
- GridSearchCV
- Sastrawi

##📌 Next Improvements
- Coba model berbasis Deep Learning (BERT/LSTM)
- Perbaiki imbalance data
- Tambah dataset forum yang lebih luas
