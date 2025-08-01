# Analisis Data Penjualan dan Rating Buku

Proyek ini bertujuan untuk melakukan analisis eksplorasi data (EDA) pada dataset "Books Sales and Ratings" dari Kaggle. Tujuannya adalah untuk mengungkap pola dan wawasan terkait faktor-faktor yang mempengaruhi popularitas dan persepsi kualitas sebuah buku.

**Link Dataset:** [Books Sales and Ratings](https://www.kaggle.com/datasets/thedevastator/books-sales-and-ratings)

## Kesimpulan & Rekomendasi

### Ringkasan Eksekutif

Analisis ini menemukan bahwa **jumlah review (`Book_ratings_count`) adalah prediktor popularitas yang lebih kuat daripada rating rata-rata (`Book_average_rating`) itu sendiri.** Genre buku dan tingkat kesulitan bahasa (`Author_Rating`) juga menunjukkan korelasi yang signifikan terhadap persepsi pembaca. Wawasan ini menyarankan bahwa strategi pemasaran yang berfokus pada perolehan review awal lebih berdampak daripada hanya menargetkan rating yang sempurna.

### Temuan Kunci (Key Insights)

*   **Popularitas vs Kualitas:** Terdapat hubungan positif yang kuat antara jumlah rating dan rating rata-rata, namun banyak buku "permata tersembunyi" (rating tinggi, jumlah rating rendah) teridentifikasi. Buku dengan lebih dari 100,000 review hampir tidak pernah memiliki rating di bawah 3.7.
*   **Dominasi Genre Tertentu:** Genre seperti "Fiction" dan "Fantasy" secara konsisten mendominasi daftar buku dengan jumlah review terbanyak. Namun, genre *niche* seperti "Historical Fiction" menunjukkan rata-rata rating tertinggi, mengindikasikan basis penggemar yang solid dan kritis.
*   **Pengaruh Tingkat Bahasa:** Buku yang ditulis oleh penulis dengan rating "Intermediate" atau "Expert" cenderung memiliki rating rata-rata yang lebih tinggi secara signifikan dibandingkan dengan "Novice", menunjukkan bahwa pembaca menghargai kompleksitas dan kedalaman tulisan.
*   **Tren Tahun Terbit:** Ada lonjakan eksponensial dalam jumlah buku yang diterbitkan setelah tahun 2000. Buku-buku modern ini mengumpulkan review lebih cepat, tetapi persaingan yang ketat membuat rata-rata rating sedikit menurun dibandingkan buku-buku klasik pra-2000.

### Rekomendasi Strategis

Berdasarkan temuan di atas, berikut adalah beberapa rekomendasi untuk para pemangku kepentingan di industri perbukuan:

*   **Untuk Penerbit & Tim Pemasaran:**
    *   **Fokus pada Review Awal:** Prioritaskan kampanye *early-reviewer* (misalnya melalui Goodreads atau NetGalley). Mendapatkan 1.000 review pertama lebih krusial untuk momentum jangka panjang daripada menunggu ulasan organik.
    *   **Investasi pada Genre Niche:** Jangan abaikan genre dengan volume rendah tetapi rating tinggi. Audiens ini sangat setia dan dapat menjadi target pemasaran yang efisien.

*   **Untuk Penulis Baru:**
    *   **Kolaborasi untuk Kredibilitas:** Jika Anda seorang penulis "Novice", berkolaborasi dengan penulis yang lebih berpengalaman atau mendapatkan editor yang kuat dapat meningkatkan persepsi kualitas karya Anda secara signifikan.
    *   **Manajemen Ekspektasi:** Memahami bahwa membangun jumlah review membutuhkan waktu adalah kunci. Fokus pada penulisan berkualitas untuk audiens spesifik Anda.

### Limitasi dan Langkah Selanjutnya

*   **Limitasi:** Dataset ini tidak memiliki informasi harga, sehingga analisis profitabilitas tidak dapat dilakukan. Selain itu, "genre" terkadang bersifat subjektif dan bisa tumpang tindih.
*   **Langkah Selanjutnya:**
    1.  Melakukan **analisis sentimen** pada sampel ulasan teks untuk memahami *alasan* di balik rating (misalnya, apa yang membuat pembaca suka/tidak suka dengan plot, karakter, dll).
    2.  Menggunakan **web scraping** untuk mendapatkan data harga dan menghubungkannya dengan data saat ini untuk membangun model prediksi pendapatan.