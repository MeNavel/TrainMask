# Train Mask

Deteksi masker menggunakan python

## Table of contents

- [Requirements](#requirements)
- [Keterangan](#keterangan)
- [Cara Menjalankan](#cara-menjalankan)


## Requirements

Development menggunakan Mac OS

- <a href="https://www.notion.so/Creating-Virtual-Environment-on-Mac-c251220eb210400f9d01eee3d5980237">Virtual Environment</a>
- <a href="https://jupyter.org/install">Jupyter Lab</a>
- <a href="https://scikit-learn.org/stable/install.html">Scikit-Learn</a>
- <a href="https://pypi.org/project/numpy/">Numpy</a>
- <a href="https://pypi.org/project/keras/">Keras</a>
- <a href="https://pypi.org/project/tensorflow/">Tensorflow</a>


## Keterangan

**Susunan dataset**

```text
dataset/
├── nama/
│    ├── mask/
│    └── no_mask/
└── nama/
    ├── mask/
    └── no_mask/

```   
Dataset berisi kumpulan folder nama orang, setiap folder nama orang berisi dua folder yaitu mask dan no_mask, yang menandakan foto tersebut ditujukan untuk seseorang yang menggunakan masker, dan tidak menggunakan masker
        
**Direktori Dataset**
```python
path = "./dataset"
```
Ubah lokasi sesuai dengan posisi dataset yang akan digunakan

**Split Data**
```python
sss = StratifiedShuffleSplit(n_splits=1, test_size=0.5, random_state=0)
```
Untuk kebutuhan split dataset yang nantinya akan ditrain
- n_splits untuk membagi data sesuai dengan nilai yang dimasukkan
- test_size untuk membagi jumlah data pada setiap split sesuai dengan persentase yang dimasukkan

## Cara Menjalankan
- Buat virtual environment
- Install requirements
- Buka Jupyter
- Klik tombol run
