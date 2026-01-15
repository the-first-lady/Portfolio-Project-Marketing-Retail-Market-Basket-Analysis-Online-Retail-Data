# Market Basket Analysis_Online Retail Data

## Overview
Proyek ini bertujuan untuk melakukan analisis keranjang pasar (Market Basket Analysis) pada data penjualan retail online. Analisis ini bertujuan untuk menemukan pola asosiasi antara produk-produk yang sering dibeli bersama, yang dapat digunakan untuk berbagai tujuan, seperti penempatan produk, rekomendasi produk, dan strategi pemasaran.

## Dataset
Dataset yang digunakan dalam analisis ini adalah **Data Retail Online**, yang berisi data transaksi dari perusahaan ritel online yang berbasis di Inggris dari tahun 2010 hingga 2011. Dataset ini mencakup kolom-kolom berikut:
- `order_id`: Identifikasi unik untuk setiap pesanan.
- `product_code`: Kode yang mewakili setiap produk.
- `product_name`: Nama produk.
- `quantity`: Jumlah produk yang dipesan.
- `order_date`: Tanggal dan waktu ketika pesanan dibuat.
- `price`: Harga per unit produk.
- `customer_id`: Identifikasi unik untuk setiap pelanggan.

- **File**: `Online Retail Data.csv`
- **Ukuran**: 32.5 MB

## Requirements
Berikut adalah beberapa pustaka Python yang diperlukan untuk menjalankan proyek ini:
- pandas
- numpy
- mlxtend
- matplotlib
- seaborn

## Langkah-langkah Analisis
Proses analisis dalam proyek ini melibatkan beberapa langkah utama:
1. **Data Preprocessing**:
   - Memuat dataset dan melakukan pembersihan data.
   - Membuat tabel pivot untuk mengkodekan transaksi.

2. **Encoding Data**:
   - Mengubah data transaksi menjadi format Boolean (True/False) untuk analisis asosiasi.

3. **Frequent Itemsets**:
   - Menggunakan algoritma Apriori untuk menemukan itemsets yang sering muncul bersama.

4. **Association Rules**:
   - Menghitung aturan asosiasi berdasarkan frequent itemsets.
   - Menghitung nilai support, confidence, dan lift dari setiap aturan asosiasi.

5. **Insights**:
   - Menyediakan wawasan dari hasil analisis asosiasi untuk pengambilan keputusan.

## Insights
Beberapa wawasan yang didapat dari analisis asosiasi produk meliputi:
- Identifikasi produk yang sering dibeli bersama.
- Peluang untuk bundling produk.
- Rekomendasi produk berdasarkan pola pembelian.
- Optimalisasi tata letak toko dan strategi pemasaran.


**Here’s a concise one-page summary table of your Market Basket Analysis insights — it highlights product pairs, confidence, lift, and the business implications in a clear, slide-ready format.**  

---

## 📊 Market Basket Analysis – Summary Table  

| **Product Pair** | **Confidence** | **Lift** | **Business Implication** |
|------------------|----------------|----------|---------------------------|
| Red heart t-light → White heart t-light | **77.22%** | **4.29** | Strong product link, cross-selling opportunity |
| Sweetheart trinket box → Strawberry trinket box | **76.19%** | **12.21** | Strong bundling potential |
| Spaceboy bag → Pink spotted bag | **72.58%** | **10.22** | Frequently bought together, bundling opportunity |
| Blue felt box → Cream felt box | **72.55%** | **14.57** | Strong link, same customer segment |
| Strawberry Charlotte bag → Red Spotty Charlotte bag | **79.55%** | **18.15** | Excellent bundling potential |
| Suki storage bag → Vintage red paisley shopper | **72.73%** | **11.65** | Marketing strategy focus |
| Lush green ribbons → Bright blue ribbons | N/A | **High** | Trend insight, strong customer preference |

---

### 🔑 Key Takeaways
- **High confidence + lift** pairs are ideal for **bundling** and **cross-selling**.  
- **Craft and bag products** show strong associations, suggesting targeted marketing for specific customer segments.  
- **Ribbon trends** highlight evolving customer preferences, useful for inventory and product design decisions.  
