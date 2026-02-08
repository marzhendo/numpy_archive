# NumPy Archive - Dokumentasi Pembelajaran

Repository ini berisi kumpulan notebook Jupyter untuk mempelajari library NumPy dalam Python.

---

## Struktur Folder

```
numpy_archive/
├── chapter-1/          # Dasar NumPy
│   ├── 2d_array.ipynb
│   ├── jam_tidur.ipynb
│   ├── latihan.ipynb
│   ├── number_of_notification.ipynb
│   └── populations.ipynb
└── chapter-2/          # NumPy Lanjutan
    ├── buildings.ipynb
    ├── hailey_comet.ipynb
    ├── langkah.ipynb
    └── titanics.ipynb
```

---

## Evaluasi Materi per Chapter

### Chapter 1: Dasar-Dasar NumPy

| Notebook | Topik | Konsep yang Dipelajari |
|----------|-------|------------------------|
| **latihan.ipynb** | Pengenalan Array | Import NumPy, pembuatan array dari list, operasi element-wise (penjumlahan array) |
| **number_of_notification.ipynb** | Agregasi Dasar | `np.sum()` untuk menjumlahkan elemen array |
| **jam_tidur.ipynb** | Array 1D & Visualisasi | `np.mean()`, `np.arange()`, indexing negatif, visualisasi dengan Matplotlib |
| **populations.ipynb** | Slicing Array | Sintaks slicing `[start:stop:step]`, indexing positif & negatif, membalik array `[::-1]` |
| **2d_array.ipynb** | Array 2D | Pembuatan array 2D, `np.mean()`, `np.min()`, `np.argmin()`, `np.unravel_index()`, masking/filtering, `np.vstack()`, `np.hstack()`, `reshape()`, `.shape`, `.size`, `.ndim` |

**Ringkasan Chapter 1:**
- Pembuatan array 1D dan 2D
- Operasi agregasi dasar: `sum()`, `mean()`, `min()`, `max()`
- Teknik slicing dan indexing
- Penggabungan array vertikal dan horizontal
- Pengubahan bentuk array dengan `reshape()`
- Visualisasi data dengan Matplotlib

---

### Chapter 2: NumPy Lanjutan

| Notebook | Topik | Konsep yang Dipelajari |
|----------|-------|------------------------|
| **buildings.ipynb** | Operasi Aritmatika | Broadcasting, operasi matematika (`+`, `-`, `*`, `/`, `**`, `%`) pada array |
| **hailey_comet.ipynb** | Generasi Array | `np.arange(start, stop, step)`, `.shape`, `reshape()` |
| **langkah.ipynb** | Agregasi dengan Axis | `np.min()`, `np.max()`, `np.mean()`, `np.sum()`, parameter `axis=0` dan `axis=1`, visualisasi line plot |
| **titanics.ipynb** | Analisis Data 2D | Array 2D kompleks, `np.argmax()`, `np.argmin()`, filtering dengan boolean masking, analisis data per kategori, visualisasi scatter plot |

**Ringkasan Chapter 2:**
- Operasi aritmatika dan broadcasting
- Penggunaan parameter `axis` untuk agregasi per baris/kolom
- Boolean masking untuk filtering data
- Analisis data berbasis kondisi
- Visualisasi data lebih kompleks

---

## Konsep NumPy yang Sudah Dikuasai

### Pembuatan Array
- [x] `np.array()` - dari list Python
- [x] `np.arange()` - array dengan interval tertentu

### Atribut Array
- [x] `.shape` - dimensi array
- [x] `.size` - jumlah total elemen
- [x] `.ndim` - jumlah dimensi

### Operasi Agregasi
- [x] `np.sum()` - penjumlahan
- [x] `np.mean()` - rata-rata
- [x] `np.min()` / `np.max()` - nilai minimum/maksimum
- [x] `np.argmin()` / `np.argmax()` - index nilai min/max
- [x] Parameter `axis` untuk agregasi per baris/kolom

### Manipulasi Array
- [x] Slicing: `[start:stop:step]`
- [x] Indexing positif dan negatif
- [x] `reshape()` - mengubah bentuk array
- [x] `np.vstack()` - penggabungan vertikal
- [x] `np.hstack()` - penggabungan horizontal
- [x] `np.unravel_index()` - konversi flat index ke multi-dimensional

### Operasi Aritmatika
- [x] Broadcasting (operasi dengan skalar)
- [x] Element-wise operations (+, -, *, /, **, %)

### Filtering & Masking
- [x] Boolean indexing
- [x] Filtering berdasarkan kondisi

### Visualisasi (dengan Matplotlib)
- [x] Line plot (`plt.plot()`)
- [x] Scatter plot (`plt.scatter()`)
- [x] Horizontal line (`plt.axhline()`)

---

## Saran Pembelajaran Selanjutnya

Berikut konsep NumPy yang belum tercakup dan bisa dipelajari:

### Level Menengah
- [ ] `np.zeros()`, `np.ones()`, `np.full()` - pembuatan array dengan nilai konstan
- [ ] `np.linspace()` - array dengan jumlah elemen tertentu
- [ ] `np.random` - pembuatan array random
- [ ] `np.sort()`, `np.argsort()` - pengurutan array
- [ ] `np.unique()` - mencari nilai unik
- [ ] `np.where()` - conditional selection
- [ ] `np.concatenate()` - penggabungan array lebih fleksibel
- [ ] `np.split()` - memecah array
- [ ] `np.std()`, `np.var()` - standar deviasi dan varians

### Level Lanjutan
- [ ] `np.dot()`, `@` operator - perkalian matriks
- [ ] `np.linalg` - operasi linear algebra
- [ ] `np.transpose()` - transposisi array
- [ ] `np.save()`, `np.load()` - menyimpan dan memuat array
- [ ] `np.genfromtxt()`, `np.loadtxt()` - membaca data dari file
- [ ] Fancy indexing dengan array integer
- [ ] `np.meshgrid()` - membuat grid koordinat
- [ ] `np.broadcast_to()` - broadcasting manual

---

## Catatan Evaluasi

### Kelebihan
1. **Pembelajaran bertahap** - Dimulai dari konsep dasar ke yang lebih kompleks
2. **Studi kasus praktis** - Menggunakan contoh nyata (populasi, jam tidur, langkah kaki, data Titanic)
3. **Visualisasi** - Menggabungkan NumPy dengan Matplotlib untuk pemahaman visual
4. **Komentar berbahasa Indonesia** - Memudahkan pemahaman

### Area yang Bisa Ditingkatkan
1. Tambahkan lebih banyak **markdown cells** untuk penjelasan teori
2. Eksplorasi **operasi linear algebra** untuk penggunaan data science
3. Praktik dengan **dataset eksternal** (CSV files)
4. Tambahkan **exercise/latihan mandiri** di setiap akhir notebook

---

## Dependencies

```python
numpy
matplotlib
```

## Quick Start

```python
import numpy as np
import matplotlib.pyplot as plt

# Contoh pembuatan array
arr = np.array([1, 2, 3, 4, 5])
print(f"Mean: {np.mean(arr)}")
print(f"Sum: {np.sum(arr)}")
```

---

*Repository ini merupakan arsip pembelajaran NumPy.*
