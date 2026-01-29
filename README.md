# Klasifikasi-Jenis-Obat
# Klasifikasi Jenis Obat (Drug Classification) 💊

Project ini bertujuan untuk membangun model *Machine Learning* yang dapat memprediksi jenis obat yang tepat untuk pasien berdasarkan metrik kesehatan tertentu. Project ini menggunakan dataset publik "Drug Classification" dan mengimplementasikan alur kerja data science mulai dari eksplorasi data (EDA), pra-pemrosesan, hingga evaluasi model.

## 📊 Tentang Dataset

Dataset yang digunakan dalam project ini bersumber dari Kaggle: [Drug Classification Dataset](https://www.kaggle.com/datasets/prathamtripathi/drug-classification/data).

Dataset ini berisi data medis pasien dengan atribut berikut yang digunakan untuk memprediksi kelas obat:

### Fitur (Features):
1.  **Age**: Umur pasien (Numerik).
2.  **Sex**: Jenis kelamin pasien (`M` = Male, `F` = Female).
3.  **BP**: Tingkat tekanan darah (`HIGH`, `NORMAL`, `LOW`).
4.  **Cholesterol**: Tingkat kolesterol (`HIGH`, `NORMAL`).
5.  **Na_to_K**: Rasio Natrium (Sodium) terhadap Kalium (Potassium) dalam darah.

### Target:
* **Drug**: Jenis obat yang diklasifikasikan (`DrugY`, `drugC`, `drugX`, `drugA`, `drugB`).

## 🚀 Fitur Utama Project

* **Exploratory Data Analysis (EDA)**: Visualisasi distribusi data pasien (sebaran umur, jenis kelamin, tekanan darah) dan korelasinya dengan jenis obat.
* **Data Preprocessing**:
    * Encoding variabel kategorikal (Label Encoding / One-Hot Encoding) untuk fitur seperti `Sex`, `BP`, dan `Cholesterol`.
    * Handling data numerik.
* **Model Training**: Pelatihan model klasifikasi (contoh: *Decision Tree*, *Random Forest*, *SVM*, atau *K-Nearest Neighbors*) untuk memprediksi kategori obat.
* **Evaluasi Model**: Pengukuran performa model menggunakan metrik akurasi (*Accuracy Score*), *Confusion Matrix*, dan *Classification Report*.

## 🛠 Teknologi yang Digunakan

Project ini dibangun menggunakan bahasa pemrograman **Python** dengan library utama sebagai berikut:

* **Pandas**: Manipulasi dan analisis data tabular.
* **NumPy**: Komputasi numerik.
* **Matplotlib & Seaborn**: Visualisasi data.
* **Scikit-Learn**: Membangun model *machine learning* dan evaluasi.
* **Jupyter Notebook**: Lingkungan interaktif untuk menjalankan kode.

## 📋 Prasyarat Instalasi

Pastikan Anda telah menginstal **Python 3.x**. Disarankan untuk menggunakan *virtual environment*.

1.  **Clone repository ini:**
    ```bash
    git clone [https://github.com/DaffaPmgks/Klasifikasi-Jenis-Obat.git](https://github.com/DaffaPmgks/Klasifikasi-Jenis-Obat.git)
    cd Klasifikasi-Jenis-Obat
    ```

2.  **Instal library yang dibutuhkan:**
    Anda dapat menginstal dependensi menggunakan `pip`. Jika terdapat file `requirements.txt`:
    ```bash
    pip install -r requirements.txt
    ```
    
    Atau instal secara manual library utama:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn jupyter
    ```

## 📂 Susunan Project

Struktur direktori project ini adalah sebagai berikut:

```text
Klasifikasi-Jenis-Obat/
├── data/
│   └── drug200.csv          # File dataset (unduh dari Kaggle jika tidak tersedia)
├── notebooks/
│   └── Klasifikasi_Obat.ipynb # Notebook utama berisi kode analisis & model
├── images/                  # (Opsional) Menyimpan hasil plot/visualisasi
├── README.md                # Dokumentasi project
└── requirements.txt         # Daftar dependensi library
