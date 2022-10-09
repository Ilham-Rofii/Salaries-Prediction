# Salaries-Prediction
## Overview
Website bernama salaries.ai-job.net adalah website yang memberikan kesempatan untuk data scientist di seluruh dunia untuk memasukkan data pendapatan mereka kedalam website tersebut. Data ini bisa digunakan oleh berbagai pihak yang membutuhkan, sehingga terwujud keterbukaaan dan transparansi data pendapatan data scientist. Project ini menggunakan data tersebut untuk memodelkan algoritma machine learning yang bisa menentukan kemungkinan pendapatan seorang data scientist.
## Data Description
Berikut ini adalah deskripsi tiap kolom yang ada dalam data:
- work_year: tahun saat menerima gaji
- experience_level: tingkat pengalaman "data scientist" yang terdiri dari EN(Entry-level/Junior), Ml(Midlevel/Intermediate), SE(Senior-level/Expert), EX(Executive-level/Director)
- employment_type: jenis kontrak kerja, PT(Part-time), FT(Full-time), CT(Contract), FL(Freelance)
- job_title: jenis pekerjaan yang dikerjakan ditahun tersebut
- salary: jumlah gaji kotor
- salary_curency: mata uang gaji yang dibayarkan
- salaryinusd: jumlah gaji dikonversikan ke USD dengan kurs tahun diterimanya gaji
- employee_residence: kode negara "data scientist" dalam ISO 3166
- remote_ratio: rasio pekerjaan yang dikerjakan secara "remote", 0(dibawah 20% "remote"), 50 (setengah "remote"), 100("remote" total)
- company_location: kode lokasi kantor "data scientist" dalam ISO 3166
- company_size: jumlah rata-rata pekerja di perusahaan pada tahun itu, S(pekerja dibawah 50 orang), M(jumlah pekerja antara 50-250 orang), L(jumlah pekerja diatas 250 orang)
## Statistical Summary
- Gaji rata-rata data scientist yang mengisi survey di website ini adalah 119266.4 USD (Sekitar 120,000 USD)
- Kebanyakan data scientist yang mengisi survey adalah data scientist senior, bekerja full time, tinggal di USA, dan bekerja di perusahaan dengan ukuran 50-250 orang yang juga berlokasi di USA
- Kebanyakan data gaji yang diisikan adalah data gaji yang diterima pada tahun 2021
## Data Modeling
- Model machine learning yang digunakan untuk memprediksi gaji dari fitur-fitur dalam data adalah polynomial regression dengan n_degree = 2
- Performa model machine learning tersebut adalah sebagai berikut:
  - RMSE = 47476.23655142554
  - MAE = 35502.92443277184
  - MAPE = 0.6640706523502142%
  - Rentang nilai target variable = 2324 USD - 600,000 USD
