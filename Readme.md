# Autoencoder Fashion-MNIST

## Nama : Zahra Arayanindra Arum Samudra

NIM : 452024618068

===

\---

## Versi Python dan Library yang Digunakan

Python : 3.12

Library:

* PyTorch
* Torchvision
* Pandas
* NumPy
* Matplotlib
* Pillow

\---

## Cara Menjalankan Training di Kaggle

1. Buka Kaggle Notebook.
2. Tambahkan dataset Fashion-MNIST.
3. Jalankan seluruh cell notebook.
4. Training dilakukan untuk latent dimension 2, 8, dan 32.
5. Setelah training selesai, simpan model menggunakan:

```python
torch.save(model.state\_dict(), "autoencoder\_32.pth")
```

6. Download file model (.pth) dari folder Output Kaggle.

\---

## Cara Menjalankan Rekonstruksi dari Terminal

1. Pastikan file berikut berada dalam satu folder:

   * reconstruct.py
   * autoencoder\_32.pth
2. Buka Command Prompt (CMD) atau Terminal.
3. Pindah ke folder project:

```bash
cd nama\_folder\_project
```

4. Jalankan program:

```bash
python reconstruct.py --model autoencoder\_32.pth --index 10
```

\---

## Contoh Perintah Terminal

```bash
python reconstruct.py --model autoencoder\_32.pth --index 10
```

atau

```bash
python reconstruct.py --model autoencoder\_8.pth --index 25
```

atau

```bash
python reconstruct.py --model autoencoder\_2.pth --index 50
```

\---

## Daftar File Output yang Dihasilkan

* autoencoder\_fashion\_mnist\_2.pth
* autoencoder\_fashion\_mnist\_8.pth
* autoencoder\_fashion\_mnist\_32.pth
* original.png
* reconstructed.png
* comparison.png
* reconstruct.py
* README.md
* laporan.pdf
* autoencoder-fashion-mnist.ipynb

```
```

