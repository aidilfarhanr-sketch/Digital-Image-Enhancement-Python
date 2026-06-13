# Image Enhancement OpenCV

## Deskripsi Proyek

**Image Enhancement OpenCV** adalah proyek pengolahan citra digital berbasis Python yang digunakan untuk meningkatkan kualitas visual gambar melalui beberapa teknik image enhancement. Proyek ini dibuat dalam bentuk Jupyter Notebook dengan antarmuka interaktif menggunakan `ipywidgets`, sehingga pengguna dapat mengatur parameter gambar secara langsung dan melihat perubahan hasilnya secara visual.

Proyek ini berfokus pada penyesuaian citra seperti kontras, kecerahan, gamma correction, histogram equalization, dan CLAHE. Selain itu, notebook ini juga menyediakan fitur perbandingan antara **Equalize Gray** dan **Equalize Luma** untuk melihat perbedaan hasil peningkatan citra pada gambar grayscale dan channel Luma pada ruang warna LAB.

## Tujuan Proyek

Tujuan dari proyek ini adalah untuk memahami dan menerapkan konsep dasar pengolahan citra digital, khususnya pada proses peningkatan kualitas gambar. Melalui proyek ini, pengguna dapat melihat bagaimana perubahan parameter seperti kontras, brightness, gamma, dan CLAHE memengaruhi tampilan citra.

## Fitur Utama

- Upload atau pilih gambar dari komputer menggunakan File Explorer.
- Mendukung format gambar seperti JPG, JPEG, PNG, BMP, TIFF, dan WEBP.
- Menampilkan perbandingan gambar asli dan gambar hasil pengolahan.
- Mengatur kontras gambar menggunakan parameter alpha.
- Mengatur kecerahan gambar menggunakan parameter beta.
- Mengatur pencahayaan gambar menggunakan gamma correction.
- Menerapkan Histogram Equalization pada gambar grayscale.
- Menerapkan Histogram Equalization pada channel Luma menggunakan ruang warna LAB.
- Menerapkan CLAHE untuk peningkatan kontras lokal.
- Mengatur nilai CLAHE clip limit.
- Mengatur ukuran CLAHE tile grid.
- Membandingkan hasil Equalize Gray dan Equalize Luma.
- Menampilkan grafik histogram untuk analisis distribusi intensitas pixel.
- Menggunakan widget interaktif agar proses eksperimen lebih mudah.

## Teknologi yang Digunakan

- Python
- OpenCV
- NumPy
- Matplotlib
- Tkinter
- IPython Display
- ipywidgets
- Jupyter Notebook

## Struktur File

```text
Image-Enhancement-OpenCV/
│
├── Tugaspengolahancitradigital_AIDIL_FARHAN_RARES.ipynb
└── README.md
```

## Penjelasan Singkat Alur Program

1. Program mengimpor library yang dibutuhkan seperti OpenCV, NumPy, Matplotlib, Tkinter, dan ipywidgets.
2. Pengguna memilih file gambar dari komputer melalui tombol interaktif.
3. Gambar dibaca menggunakan OpenCV dan dikonversi dari BGR ke RGB agar sesuai untuk ditampilkan dengan Matplotlib.
4. Pengguna dapat mengubah nilai kontras, brightness, gamma, CLAHE clip, dan CLAHE tile melalui slider.
5. Program memproses gambar berdasarkan parameter yang dipilih.
6. Hasil pengolahan citra ditampilkan berdampingan dengan gambar asli.
7. Pengguna dapat membandingkan metode Equalize Gray dan Equalize Luma.
8. Program menampilkan histogram sebelum dan sesudah equalization untuk membantu analisis visual.

## Metode Pengolahan Citra

### 1. Contrast Adjustment

Kontras digunakan untuk mengatur perbedaan intensitas antara area terang dan gelap pada gambar. Pada proyek ini, kontras diatur menggunakan parameter alpha.

### 2. Brightness Adjustment

Brightness digunakan untuk mengatur tingkat kecerahan gambar. Nilai positif akan membuat gambar lebih terang, sedangkan nilai negatif akan membuat gambar lebih gelap.

### 3. Gamma Correction

Gamma correction digunakan untuk mengatur pencahayaan gambar secara non-linear. Teknik ini berguna untuk memperbaiki gambar yang terlalu gelap atau terlalu terang.

### 4. Histogram Equalization Grayscale

Metode ini dilakukan pada gambar grayscale untuk meratakan distribusi intensitas pixel sehingga kontras gambar dapat meningkat.

### 5. Equalization pada Luma

Metode ini dilakukan pada channel L dari ruang warna LAB. Pendekatan ini dapat meningkatkan kontras pencahayaan tanpa terlalu merusak informasi warna pada gambar.

### 6. CLAHE

CLAHE atau Contrast Limited Adaptive Histogram Equalization digunakan untuk meningkatkan kontras lokal pada gambar. Metode ini lebih terkontrol dibandingkan histogram equalization global karena menggunakan pembagian area kecil atau tile.

## Parameter Interaktif

| Parameter | Fungsi |
|---|---|
| Contrast Alpha | Mengatur tingkat kontras gambar |
| Brightness Beta | Mengatur tingkat kecerahan gambar |
| Gamma | Mengatur pencahayaan non-linear |
| Equalization | Memilih mode None, Gray, atau Luma |
| CLAHE Clip | Mengatur batas peningkatan kontras lokal |
| CLAHE Tile | Mengatur ukuran area lokal untuk proses CLAHE |

## Cara Menjalankan Proyek

1. Clone repository ini:

```bash
git clone https://github.com/username/Image-Enhancement-OpenCV.git
```

2. Masuk ke folder project:

```bash
cd Image-Enhancement-OpenCV
```

3. Install library yang dibutuhkan:

```bash
pip install opencv-python numpy matplotlib ipywidgets
```

4. Jalankan Jupyter Notebook:

```bash
jupyter notebook
```

5. Buka file notebook:

```text
Tugaspengolahancitradigital_AIDIL_FARHAN_RARES.ipynb
```

6. Jalankan setiap cell secara berurutan.

7. Klik tombol **Pilih File Foto**, lalu pilih gambar yang ingin diproses.

## Contoh Penggunaan

- Meningkatkan kontras gambar yang terlihat gelap.
- Mengatur brightness pada gambar underexposed atau overexposed.
- Membandingkan hasil equalization pada grayscale dan luma.
- Menganalisis distribusi intensitas pixel melalui histogram.
- Mempelajari efek CLAHE terhadap detail gambar.

## Hasil yang Diharapkan

Hasil dari proyek ini adalah pengguna dapat memahami bagaimana teknik image enhancement bekerja pada gambar digital. Pengguna juga dapat melihat secara langsung perubahan visual yang terjadi ketika parameter pengolahan citra diubah.

## Manfaat Proyek

- Membantu memahami dasar pengolahan citra digital.
- Cocok untuk tugas kuliah, praktikum, dan portofolio.
- Menunjukkan penerapan OpenCV dalam manipulasi gambar.
- Memberikan gambaran visual tentang histogram equalization dan CLAHE.
- Menjadi dasar untuk pengembangan aplikasi computer vision yang lebih kompleks.

## Author

**Aidil Farhan Rares**

## Lisensi

Proyek ini dibuat untuk kebutuhan pembelajaran, tugas, dan portofolio. Silakan digunakan sebagai referensi dengan tetap mencantumkan sumber atau pembuat asli.
