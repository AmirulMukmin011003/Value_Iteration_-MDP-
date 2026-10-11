# Implementasi Value Iteration pada Markov Decision Process (MDP)

## Deskripsi

Repository ini berisi implementasi algoritma **Value Iteration** untuk menyelesaikan permasalahan pengambilan keputusan menggunakan *Markov Decision Process* (MDP). Eksperimen dilakukan menggunakan Python untuk menghitung nilai optimal setiap state dan menentukan kebijakan optimal (*optimal policy*) berdasarkan reward, faktor diskonto, dan batas toleransi konvergensi.

## Tujuan

- Memahami konsep Markov Decision Process (MDP).
- Mengimplementasikan algoritma Value Iteration menggunakan Python.
- Menghitung nilai optimal pada setiap state.
- Menentukan kebijakan optimal berdasarkan nilai setiap tindakan.
- Menganalisis pengaruh faktor diskonto terhadap hasil iterasi.

## Daftar Eksperimen

| File | Studi Kasus |
|---|---|
| `VI.ipynb` | Eksperimen 1: Implementasi dasar Value Iteration |
| `VI_EKS2.ipynb` | Eksperimen 2: Perjalanan dari rumah ke kampus dengan faktor diskonto 0,9 |
| `VI_EKS3.ipynb` | Eksperimen 3: Studi kasus perjalanan dari rumah ke kampus dengan faktor diskonto 0,5 |

## Metode

Algoritma Value Iteration memperbarui nilai setiap state berdasarkan reward langsung dan nilai state tujuan yang telah didiskontokan.

Persamaan Bellman optimality yang digunakan adalah:

\[
V_{k+1}(s)=\max_a\left[R(s,a,s')+\gamma V_k(s')\right]
\]

Keterangan:
- \(V_{k+1}(s)\): nilai state pada iterasi berikutnya.
- \(R(s,a,s')\): reward dari tindakan yang dipilih.
- \(\gamma\): faktor diskonto.
- \(V_k(s')\): nilai state tujuan pada iterasi sebelumnya.
- \(\max_a\): memilih tindakan dengan nilai terbesar.

Iterasi dihentikan ketika perubahan nilai maksimum antaritersi lebih kecil daripada batas toleransi yang ditentukan.

## Teknologi

- Python
- Jupyter Notebook
- Matplotlib (untuk visualisasi hasil iterasi)

## Cara Menjalankan

1. Clone repository ini:

   ```bash
   git clone https://github.com/AmirulMukmin011003/Value_iteration_MDP.git
   ```

2. Masuk ke direktori repository:

   ```bash
   cd Value_iteration_MDP
   ```

3. Instal pustaka yang diperlukan:

   ```bash
   pip install matplotlib notebook
   ```

4. Jalankan Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Buka salah satu file eksperimen (`VI.ipynb`, `VI_EKS2.ipynb`, atau `VI_EKS3.ipynb`) dan jalankan sel secara berurutan.

## Hasil Eksperimen

Hasil eksperimen mencakup nilai optimal setiap state, kebijakan optimal, jumlah iterasi hingga konvergensi, serta visualisasi perubahan nilai state jika tersedia pada notebook.

## Penulis

**Amirul Mukmin**

Repository ini dibuat untuk keperluan pembelajaran dan implementasi algoritma kecerdasan buatan, khususnya Value Iteration pada MDP.
