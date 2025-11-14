# netflix-data-analysis

Netflix merupakan salah satu platform streaming terbesar di dunia yang menawarkan ribuan konten film dan serial dari berbagai negara. Dataset yang digunakan dalam proyek ini berisi informasi detail mengenai setiap konten—mulai dari judul, sutradara, negara asal, tahun rilis, hingga genre.

Tujuan dari analisis ini adalah untuk:

Memahami distribusi konten berdasarkan jenis (Movie/TV Show), tahun rilis, negara, rating, dan genre.

Mengidentifikasi tren penambahan konten dari waktu ke waktu.

Melakukan eksplorasi mendalam mengenai karakteristik Movie & TV Show di Netflix.

Menghasilkan insight strategis terkait pola dan preferensi konten Netflix secara global.

📌 Data Understanding & Cleaning

Pada tahap awal dilakukan beberapa proses untuk memahami dan mempersiapkan data:

✔ Memeriksa struktur data (df.info())

Dataset berisi 8.807 baris dan 12 kolom.

Beberapa kolom penting berupa teks: title, director, cast, country, listed_in.

Kolom tanggal seperti date_added membutuhkan konversi ke datetime.

✔ Memeriksa nilai unik (df.nunique())

Hasil pengamatan awal:

4.528 sutradara berbeda → menunjukkan keberagaman kreator.

7.692 aktor terlibat dalam berbagai konten.

748 negara tercatat → Netflix benar-benar global.

17 kategori rating → digunakan untuk segmentasi umur dan regulasi konten.

✔ Menangani Missing Value

Beberapa kolom memiliki missing values cukup besar, terutama:

director

cast

country

date_added

rating

duration

Missing value ditangani dengan pendekatan:

Tetap dibiarkan "Unknown" untuk kolom kategori → tidak merusak distribusi.

date_added dikonversi menjadi datetime dan missing tidak dipaksakan.

📌 Dataset Overview

Dataset terdiri dari:

8.807 baris

12 kolom

Konten dibagi menjadi Movie dan TV Show

Rentang tahun rilis: 1925 → 2021

📌 Insight penting:
Dataset ini tidak memiliki konten rilis di atas tahun 2021, sehingga tren yang dianalisis hanya berlaku hingga 2021.
Artinya, perubahan strategi Netflix pada 2022–2025 tidak tercakup, dan interpretasi harus mempertimbangkan hal ini.

📌 Rekomendasi Perbaikan (Supaya Portofolio Semakin Profesional)

✔ Tambahkan visualisasi distplot/histogram untuk tahun rilis.
✔ Tambahkan barplot untuk Movie vs TV Show.
✔ Lakukan Top Countries analysis (10 besar negara paling produktif).
✔ Lakukan WordCloud untuk genre (opsional tapi menarik di GitHub).
✔ Buat section Key Insights & Conclusion.

🎯 Key Insights 

International Movies mendominasi genre → menunjukkan fokus Netflix pada pasar global.

Kids TV hanya berjumlah < 500 konten → Netflix lebih banyak menyediakan konten dewasa dan keluarga, bukan fokus anak.

Tren rilis meningkat tajam setelah 2015 → sejalan dengan ekspansi global Netflix.

Countries sangat beragam (748 negara) → bukti kuat bahwa Netflix bukan hanya Hollywood-centric.

Rating TV-MA mendominasi → konten dewasa paling banyak ditonton sehingga produksinya paling besar.

🏁 Conclusion

Analisis ini memberikan gambaran menyeluruh mengenai konten Netflix. Dari hasil eksplorasi data, dapat disimpulkan:

Netflix menargetkan pasar global, terlihat dari keberagaman negara dan dominasi International Movies.

Konten dewasa (TV-MA) dan genre Drama/Comedy merupakan yang paling banyak diproduksi.

Dataset menunjukkan peningkatan konten signifikan setelah 2015, mencerminkan ekspansi agresif Netflix.

Dataset terbatas hingga 2021 sehingga perlu sumber lain jika ingin melihat tren terbaru.
