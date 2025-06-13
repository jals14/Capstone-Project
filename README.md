# MATH LENS
OCR Angka Tulisan Tangan - Deteksi Angka dari Gambar

## 📝 Deskripsi Proyek

Proyek ini membangun sistem **OCR (Optical Character Recognition)** sederhana yang mampu mengenali **angka tulisan tangan** dari gambar. Model yang digunakan adalah **Convolutional Neural Network (CNN)** yang dilatih menggunakan dataset **MNIST**. Sistem ini disediakan melalui **REST API** menggunakan **FastAPI**, sehingga pengguna dapat mengunggah gambar dan langsung mendapatkan hasil prediksi angka.

---

## 🧠 Arsitektur Model

Model yang digunakan adalah **CNN 2D sederhana** yang memiliki struktur sebagai berikut:

1. **Input layer**: Gambar 28x28 piksel grayscale  
2. **2 Conv2D layer** dengan ReLU activation  
3. **MaxPooling layer**  
4. **Flatten layer**  
5. **Dense (fully connected) layer**  
6. **Output layer** dengan 10 neuron (kelas angka 0–9) dan softmax activation  

Model dilatih pada dataset **MNIST**, dengan preprocessing berupa:
- Grayscale conversion
- Normalisasi nilai piksel (0–1)
- Resize ke 28x28 piksel
- Reshape untuk menyesuaikan input CNN

---

## ⚙️ Teknologi yang Digunakan

- Python 3.11 
- TensorFlow / Keras  
- FastAPI  
- NumPy  
- Pillow (PIL)  
- Uvicorn (server)

---

## 📷 Cara Menggunakan
1. Extract file Capstone.zip
2. Buka folder Capstone lalu copy path foldernya
3. buka terminal/cmd kemudian ketikkan "cd "Isi dengan path folder"" lalu enter.
4. kemudian ketikkan "uvicorn main:app --reload" lalu enter
5. copy link https://.....
6. Buka endpoint /docs melalui browser.
7. Gunakan form pada endpoint /predict.
8. Upload gambar angka tulisan tangan (format .png, .jpg, dll).
9. Klik "Execute", dan sistem akan merespons prediksi angka dan confidence-nya.
  
## 🔗 Dataset
Dataset yang digunakan: MNIST (via Kaggle)

