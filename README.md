# 📊 Customer Segmentation using Length, Recency, Frequency, and Monetary (LRFM) on Superstore Dataset

## 📌 Ringkasan

Proyek ini bertujuan untuk mengelompokkan pelanggan berdasarkan perilaku pembelian mereka dengan menggunakan metode **LRFM (Length, Recency, Frequency, Monetary)**. Melalui pendekatan ini, perusahaan dapat memperoleh wawasan yang lebih dalam mengenai siklus hidup pelanggan dan menyusun strategi pemasaran yang lebih efektif dan efisien.

---

## 🔍 Metodologi

### 1. Persiapan dan Pembersihan Data
- Dataset Superstore dibersihkan dari data duplikat dan nilai kosong.
- Kolom tanggal dikonversi ke dalam format `datetime`.

### 2. Perhitungan Komponen LRFM
- **Length**: Selisih waktu antara transaksi pertama dan terakhir dari masing-masing pelanggan.
- **Recency**: Jarak waktu sejak pembelian terakhir hingga tanggal acuan analisis.
- **Frequency**: Jumlah transaksi unik yang dilakukan oleh pelanggan.
- **Monetary**: Total nilai transaksi yang dilakukan oleh pelanggan.

### 3. Skoring dan Segmentasi
- Setiap metrik LRFM diberi skor menggunakan skala kuartil.
- Skor digabungkan dan dianalisis untuk mengelompokkan pelanggan ke dalam beberapa segmen perilaku.

---

## 🧩 Segmentasi Pelanggan

Berikut adalah pembagian segmen pelanggan berdasarkan hasil analisis:

| Segmen         | Deskripsi Singkat | Temuan Utama |
|----------------|-------------------|--------------|
| **Lost**       | Pelanggan tidak lagi aktif dan mengalami penurunan frekuensi pembelian. | Penjualan tertinggi berasal dari Inggris dan Île-de-France. |
| **At Risk**    | Pelanggan dengan risiko berhenti melakukan pembelian. | Inggris merupakan pasar dengan tingkat risiko tertinggi. |
| **Hibernating**| Pelanggan jarang melakukan pembelian namun masih aktif secara sporadis. | Fokus pada produk seperti Copiers dan Phones. |
| **Need Attention** | Pelanggan yang memerlukan perhatian untuk mempertahankan loyalitas mereka. | Produk utama: Storage dan Copiers. |
| **Promising**  | Pelanggan dengan potensi pertumbuhan yang baik. | Aktivitas belanja meningkat di wilayah Lower Saxony. |
| **Loyal**      | Pelanggan setia yang secara konsisten berkontribusi terhadap pendapatan. | Produk populer: Diabolos dan Appliances. |
| **Big Spender**| Pelanggan dengan pengeluaran besar untuk kategori produk tertentu. | Produk unggulan: Phones dan Machines. |
| **Champions**  | Pelanggan terbaik yang memberikan kontribusi terbesar terhadap pendapatan perusahaan. | Inggris menjadi wilayah dominan dalam segmen ini. |

---

## ✅ Kesimpulan

- Segmentasi menggunakan pendekatan LRFM memberikan pemahaman yang komprehensif mengenai karakteristik pelanggan.
- Inggris merupakan wilayah dengan dominasi pelanggan dalam hampir semua segmen utama.
- Terdapat korelasi yang jelas antara jenis produk dengan preferensi pelanggan di setiap segmen.
- Segmen *Champions*, *Big Spenders*, dan *Loyal* merupakan segmen strategis yang perlu dipertahankan dan diberi perlakuan khusus.

---

## 💡 Rekomendasi Strategis

### 🔄 Lost
Melakukan kampanye *re-engagement* seperti diskon atau promosi produk yang sebelumnya diminati (misalnya produk *Copiers*).

### ⚠️ At Risk
Menerapkan program loyalitas atau insentif khusus untuk mendorong pembelian ulang sebelum pelanggan benar-benar berhenti bertransaksi.

### 💤 Hibernating
Mengirimkan notifikasi berkala terkait produk baru atau layanan tambahan berdasarkan riwayat pembelian sebelumnya, seperti produk *Phones*.

### 👀 Need Attention
Memberikan dukungan pelanggan yang personal dan responsif serta menawarkan solusi proaktif untuk mempertahankan hubungan jangka panjang.

### 🌱 Promising
Fokus pada pemasaran yang ditargetkan kepada kelompok demografis serupa guna meningkatkan potensi konversi menjadi pelanggan setia.

### 💎 Loyal
Menyediakan sistem penghargaan atau akses eksklusif ke program tertentu sebagai bentuk apresiasi terhadap loyalitas mereka.

### 🛍️ Big Spender
Menawarkan layanan VIP atau paket premium untuk meningkatkan pengalaman pelanggan sekaligus menjaga retensi jangka panjang.

### 🏆 Champions
Melibatkan pelanggan dalam proses *co-creation* produk untuk memperoleh wawasan pengguna langsung dan membangun rasa kepemilikan terhadap merek.

---

## 🧰 Teknologi dan Tools

- **Python**: Pandas, NumPy, Matplotlib, Seaborn
- **Jupyter Notebook / Google Colab**
- **Tableau**

