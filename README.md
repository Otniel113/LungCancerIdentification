# LungCancerIdentification
Identifikasi kanker paru-paru pada perokok menggunakan Metode Ensemble berdasarkan Data Ekspresi Gen

## Abstrak
Kanker adalah gejala pertumbuhan sel secara abnormal dan tidak terkendali. Organ tubuh yang sering diserang kanker adalah paru-paru atau disebut juga kanker paru-paru. Kanker paru-paru merupakan kanker dengan penyebab kematian tertinggi di dunia. 

Penyebab kanker paru-paru paling banyak adalah rokok. Perokok memiliki risiko terkena kanker paru-paru lebih tinggi daripada non-perokok. Deteksi dini sangat penting dilakukan karena dapat mencegah kanker paru-paru sehingga mendapatkan penanganan yang tepat. Upaya deteksi dini yang umum dilakukan adalah screening dengan menggunakan low dose CT scan (LDCT). Namun upaya ini masih memiliki kekurangan yaitu hanya dapat mendeteksi kanker pada stadium akhir dan diperlukan penanganan khusus. 

Dengan kemajuan teknologi microarray DNA (mikro-larik DNA), dapat diukur tingkat ekspresi gen dari ribuan gen atau sel dalam jaringan tertentu. Sehingga dapat dilakukan identifikasi kanker paru-paru dengan menggunakan machine learning dari data ekspresi gen (microarray DNA) tersebut. Dalam penelitian ini akan dibangun model prediksi machine learning menggunakan Metode Ensemble (Ensemble Method). Metode Ensemble yang dipakai adalah Random Forest dan AdaBoost. Metode ini dipilih karena memiliki performansi yang baik dan lebih dalam melakukan prediksi daripada dengan menggunakan model individu. 

Hasil prediksi tersebut berupa identifikasi apakah pasien memiliki kanker paru-paru atau tidak dan akan divalidasi kebenarannya menggunakan metrik akurasi.

<b>Kata kunci:</b> kanker paru-paru, perokok, metode ensemble, data ekspresi gen

## Tujuan
Tujuan pada penelitian ini adalah:
1. Mendapatkan hasil seleksi fitur yang optimal
2. Membangun model prediksi menggunakan Metode Ensemble
3. Mengetahui akurasi Metode Ensemble dalam melakukan prediksi

## Alur Pemodelan
![Alur_New_2](https://user-images.githubusercontent.com/57952404/167335117-a1cb1a7e-072a-4ddd-a4e3-a7d189e289d6.png)


## Dataset
Dataset yang digunakan berasal dari GEO (Gene Expression Omnibus) yang didapatkan dari website basis data bioteknologi NCBI (National Center of Biotechnology Information). Data seri yang digunakan adalah GSE4115, berisi data ekspresi gen dari perokok yang diduga memiliki kanker paru-paru. Data tersebut memiliki 187 sampel pasien dengan hasil diagnosis 97 pasien memiliki kanker paru-paru dan 90 pasien tidak memiliki kanker paru-paru. Dilakukan pemisahan (split) data menjadi data latih dan juga data uji. Data latih memiliki proporsi sebanyak 70% sedangkan data uji memiliki proporsi sebanyak 30%.

Source : https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE4115

