# VisionTransformer-Comparison

## Dosen Pengampu: **Martin Clinton Tosima Manullang, S.T., M.T., Ph.D** **Imam Eko Wicaksono, S.Si., M.Si.**

| **Nama**                    | **NIM**   | **ID GITHUB**                                                               |
| --------------------------- | --------- | --------------------------------------------------------------------------- |
| Shintya Ayu Wardani     | 122140138 | <a href="https://github.com/shintyawa">@shintyawa</a>                     |

---

## **Tujuan**

Menganalisis pengaruh desain arsitektur terhadap performa dengan membandingkan Vision Transformer
(ViT) dan Swin Transformer.

---

## **Alat yang Digunakan**
|**Logo**  | **Nama**   | **Fungsi**   |
| -------- |------------|--------------|
|<img src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Visual_Studio_Code_1.35_icon.svg" alt="VS Code Logo" width="70">|   VSCode   |Editor kode utama untuk menulis, mengedit, dan menjalankan skrip Python dengan fitur seperti debugging, ekstensi, dan integrasi Git.|
|<img src="https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg" alt="Python Logo" width="70">|   Python   |Sebagai bahasa pemrograman utama untuk membangun dan menjalankan logika pemrosesan sinyal, analisis data, serta antarmuka sistem.|
---
## **Library yang Digunakan**

Berikut adalah daftar library Python yang digunakan dalam proyek ini, beserta fungsinya:

- - -

| **No.** | **Library**                                                                          | **Fungsi**                                                                                        |
| ------- | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
| 1       | `os`, `pathlib.Path`                                                                 | Mengelola path dan operasi file/folder (membuat, mengecek, dan mengatur direktori/proyek).        |
| 2       | `random`                                                                             | Menghasilkan nilai acak, misalnya untuk seeding dan augmentasi acak.                              |
| 3       | `time`                                                                               | Mengukur waktu eksekusi dan memberi jeda (sleep) pada proses.                                     |
| 4       | `json`                                                                               | Membaca dan menyimpan konfigurasi atau hasil dalam format JSON.                                   |
| 5       | `math`                                                                               | Operasi matematika dasar (fungsi trigonometri, logaritma, dsb.).                                  |
| 6       | `warnings`                                                                           | Mengatur dan menampilkan peringatan selama eksekusi kode.                                         |
| 7       | `numpy`                                                                              | Komputasi numerik dan manipulasi array untuk data numerik besar.                                  |
| 8       | `pandas`                                                                             | Membaca, memproses, dan mengelola data tabular (CSV, dataframe label, dsb.).                      |
| 9       | `PIL.Image` (Pillow)                                                                 | Membaca dan memanipulasi file gambar sebelum diproses model.                                      |
| 10      | `torch`                                                                              | Library utama PyTorch untuk tensor, operasi numerik, dan eksekusi di CPU/GPU.                     |
| 11      | `torch.nn`                                                                           | Membangun arsitektur neural network (layer, loss function, dsb.).                                 |
| 12      | `torch.optim`                                                                        | Optimizer (misalnya Adam, SGD) untuk melatih model deep learning.                                 |
| 13      | `torch.utils.data.Dataset`, `DataLoader`                                             | Membuat dataset kustom dan loader mini-batch yang efisien.                                        |
| 14      | `torchvision.transforms`                                                             | Transformasi data gambar (resize, normalisasi, augmentasi dasar).                                 |
| 15      | `torchinfo.summary`                                                                  | Menampilkan ringkasan arsitektur model (jumlah parameter, ukuran output tiap layer).              |
| 16      | `timm`                                                                               | Koleksi model vision SOTA (mis. ViT, Swin) dan utilitas terkait.                                  |
| 17      | `CosineLRScheduler` dari `timm.scheduler.cosine_lr`                                  | Scheduler learning rate dengan pola cosine decay selama training.                                 |
| 18      | `albumentations`, `albumentations.pytorch.ToTensorV2`                                | Augmentasi gambar tingkat lanjut dan konversi ke tensor PyTorch.                                  |
| 19      | `matplotlib.pyplot`                                                                  | Visualisasi hasil training, kurva loss/akurasi, dan contoh prediksi.                              |
| 20      | `StratifiedKFold`, `train_test_split` dari `sklearn.model_selection`                 | Membagi data menjadi train/valid secara terstratifikasi dan acak.                                 |
| 21      | `classification_report`, `confusion_matrix`, `accuracy_score` dari `sklearn.metrics` | Menghitung metrik evaluasi klasifikasi (akurasi, precision, recall, F1, dan matriks kebingungan). |

---

## Cara Menjalankan Program

Dengan asumsi Anda sudah menginstal Python (disarankan versi 3.12), ikuti langkah-langkah berikut untuk menjalankan proyek ini:

### 1. Clone Repository

```yaml
git clone [https://github.com/shintyawa/VisionTransformer-Comparison.git]
```

### 2. Install UV

```yaml
pip install uv
```

### 3. Membuat Virtual Environment (venv)

```yaml
uv venv --python=python3.12
```

Aktifkan environment (pilih sesuai sistem operasi Anda):
- Windows :

```yaml
.venv/Scripts/activate
```

- MacOS :

```yaml
source .venv/bin/activate
```

- Linux :

```yaml
source venv/bin/activate
```
### 4. Install requirements.txt

```yaml
uv pip install -r requirements.txt
```

### 5. Jalankan program

```yaml
uv run main.py
```
