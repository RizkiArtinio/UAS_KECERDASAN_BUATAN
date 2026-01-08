# Tugas UAS Kecerdasan Buatan - Klasifikasi Spesies Iris

Project ini merupakan implementasi algoritma **Decision Tree** untuk mengklasifikasikan spesies bunga Iris berdasarkan fitur morfologinya. Tugas ini disusun untuk memenuhi ujian akhir semester pada mata kuliah Kecerdasan Buatan.

## 👤 Identitas Diri
* **Nama** : Rizki Artinio Permana Putra
* **NIM** : 231011401590
* **Kelas** : 05TPLE013

## 📝 Deskripsi Project
Project ini berfokus pada penggunaan *Machine Learning* berbasis pohon keputusan (*Decision Tree*) untuk memprediksi tiga varietas bunga Iris: **Setosa**, **Versicolor**, dan **Virginica**. 

Dataset yang digunakan mengandung 5 kolom utama:
1.  `SepalLengthCm`: Panjang Kelopak
2.  `SepalWidthCm`: Lebar Kelopak
3.  `PetalLengthCm`: Panjang Mahkota
4.  `PetalWidthCm`: Lebar Mahkota
5.  `Species`: Label target (Spesies)

Langkah-langkah yang dilakukan dalam project ini meliputi:
* **Preprocessing**: Pembersihan data dan penghapusan fitur yang tidak relevan (`Id`).
* **Data Splitting**: Pembagian data menjadi 80% data latih dan 20% data uji.
* **Modeling**: Implementasi `DecisionTreeClassifier` dengan kriteria *Gini Impurity*.
* **Visualisasi**: Penggambaran struktur pohon keputusan menggunakan `matplotlib`.

## 📊 Hasil Analisis
Berdasarkan hasil eksperimen yang dilakukan, diperoleh poin-poin analisis sebagai berikut:

1.  **Akurasi Model**: Model berhasil mencapai tingkat akurasi sebesar **100% (1.0)** pada data uji. Hal ini menunjukkan bahwa fitur-fitur pada bunga Iris memiliki pola yang sangat jelas dan dapat dipisahkan secara linear oleh algoritma.
2.  **Fitur Paling Berpengaruh**: Melalui visualisasi pohon keputusan, ditemukan bahwa `PetalLengthCm` dan `PetalWidthCm` adalah dua fitur kunci yang paling menentukan dalam proses klasifikasi.
3.  **Evaluasi**: Nilai *Precision*, *Recall*, dan *F1-Score* untuk ketiga kelas mencapai skor sempurna, menandakan model sangat stabil dan tidak mengalami *bias* pada satu spesies tertentu.
4.  **Kesimpulan**: Penggunaan parameter `max_depth=3` sudah cukup efektif untuk mendapatkan hasil yang optimal tanpa membuat model menjadi terlalu kompleks (*overfitting*).