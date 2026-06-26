# Autoencoder Fashion-MNIST

## Identitas

**Nama:** Zahra Arayanindra Arum Samudra

**NIM:** 452024618068

**Mata Kuliah:** Pembelajaran Mesin 2

---

## Deskripsi Proyek

Project ini merupakan implementasi **Convolutional Autoencoder** menggunakan **PyTorch** untuk melakukan rekonstruksi citra pada dataset **Fashion-MNIST**. Model dilatih menggunakan tiga ukuran **latent dimension** (2, 8, dan 32) untuk membandingkan kualitas hasil rekonstruksi citra.

---

## Dataset

Dataset yang digunakan adalah **Fashion-MNIST** dengan spesifikasi:

* 60.000 data training
* 10.000 data testing
* Ukuran citra 28 × 28 piksel (grayscale)
* Terdiri dari 10 kategori pakaian

---

## Versi Python dan Library

**Python:** 3.12

**Library yang digunakan:**

* PyTorch
* Torchvision
* Pandas
* NumPy
* Matplotlib
* Pillow

---

## Cara Menjalankan Training di Kaggle

1. Buka Kaggle Notebook.
2. Tambahkan dataset Fashion-MNIST.
3. Jalankan seluruh cell notebook secara berurutan.
4. Lakukan training untuk latent dimension **2**, **8**, dan **32**.
5. Setelah proses training selesai, simpan model menggunakan:

```python
torch.save(model.state_dict(), "autoencoder_fashion_mnist_32.pth")
```

6. Download file model (.pth) dari folder **Output** Kaggle.

---

## Cara Menjalankan Rekonstruksi dari Terminal

Pastikan file berikut berada dalam satu folder:

* reconstruct.py
* autoencoder_fashion_mnist_32.pth

Buka Command Prompt (CMD) atau Terminal, kemudian masuk ke folder project:

```bash
cd nama_folder_project
```

Jalankan program:

```bash
python reconstruct.py --model autoencoder_fashion_mnist_32.pth --index 10
```

---

## Contoh Perintah

Latent Dimension 32

```bash
python reconstruct.py --model autoencoder_fashion_mnist_32.pth --index 10
```

Latent Dimension 8

```bash
python reconstruct.py --model autoencoder_fashion_mnist_8.pth --index 25
```

Latent Dimension 2

```bash
python reconstruct.py --model autoencoder_fashion_mnist_2.pth --index 50
```

---

## Struktur Project

```text
├── autoencoder-fashion-mnist.ipynb
├── reconstruct.py
├── generator_from_decoder.py
├── autoencoder_fashion_mnist_2.pth
├── autoencoder_fashion_mnist_8.pth
├── autoencoder_fashion_mnist_32.pth
├── original.png
├── reconstructed.png
├── comparison.png
├── README.md
└── Laporan.pdf
```

---

## Hasil

Project berhasil melakukan proses rekonstruksi citra Fashion-MNIST menggunakan Autoencoder. Berdasarkan hasil eksperimen, semakin besar ukuran **latent dimension**, semakin baik kualitas citra hasil rekonstruksi karena model mampu menyimpan lebih banyak informasi penting pada latent space.

---

