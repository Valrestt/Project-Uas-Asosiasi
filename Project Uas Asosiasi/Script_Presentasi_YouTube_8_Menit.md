# Script Presentasi YouTube Minimal 8 Menit

Assalamualaikum warahmatullahi wabarakatuh. Perkenalkan, nama saya [isi nama] dari kelas [isi kelas]. Pada video presentasi ini, saya akan menjelaskan project UAS Data Mining dengan metode Association Rule Mining. Dataset yang saya gunakan adalah Dataset Respons Pelanggan Cafe terhadap Promo Digital. Analisis ini menggunakan framework CRISP-DM dan dua algoritma, yaitu Apriori dan FP-Growth.

Latar belakang dari project ini adalah penggunaan promo digital oleh cafe untuk menarik perhatian pelanggan. Promo digital dapat dikirim melalui beberapa channel seperti web, email, mobile, dan social media. Namun, setiap pelanggan bisa memberikan respons yang berbeda. Ada pelanggan yang hanya menerima promo, dan ada juga pelanggan yang melihat promo tersebut.

Masalah utama dalam analisis ini adalah bagaimana menemukan pola kombinasi antara karakteristik pelanggan, jenis promo, channel promo, dan event respons pelanggan. Dengan menggunakan metode asosiasi, kita dapat melihat item atau atribut apa saja yang sering muncul bersama dalam satu transaksi.

Tujuan project ini adalah menemukan association rules yang dapat membantu cafe dalam menyusun strategi promosi digital. Misalnya, cafe dapat mengetahui kombinasi jenis promo dan channel yang sering berkaitan dengan respons pelanggan tertentu.

Dataset ini terdiri dari beberapa kolom, yaitu customer_id, gender, age_group, income_group, offer_id, offer_type, difficulty_group, reward_group, duration_group, channel_web, channel_email, channel_mobile, channel_social, event, dan association_items.

Kolom yang paling penting untuk analisis asosiasi adalah association_items. Kolom ini berisi daftar item per transaksi, misalnya gender pelanggan, kelompok usia, jenis promo, reward, durasi, channel yang digunakan, dan event respons pelanggan. Karena sudah ada kolom association_items, dataset ini cocok digunakan untuk Association Rule Mining.

Pada tahap data understanding, saya menampilkan lima data pertama, lima data terakhir, informasi dataset, jumlah baris dan kolom, statistik deskriptif, nama kolom, tipe data, jumlah nilai unik, serta distribusi beberapa kolom penting seperti event dan offer_type.

Tahap berikutnya adalah data preparation. Pada tahap ini, saya membuat salinan dataset agar data asli tetap aman. Kemudian nama kolom dirapikan, missing values dicek, dan data duplikat dihapus jika ditemukan.

Setelah itu, kolom association_items diubah menjadi bentuk list transaksi. Setiap baris data dianggap sebagai satu transaksi. Kemudian list transaksi tersebut diubah menjadi bentuk one-hot encoding menggunakan TransactionEncoder. Format ini dibutuhkan agar algoritma Apriori dan FP-Growth dapat memproses data.

Saya juga mengecek item yang terlalu konstan, yaitu item yang muncul hampir di semua transaksi. Item seperti ini dapat menghasilkan rules yang kurang informatif. Oleh karena itu, item dengan support sangat tinggi dapat dihapus dari data modeling agar hasil rules lebih bermakna.

Pada tahap modeling, saya menggunakan dua algoritma, yaitu Apriori dan FP-Growth. Parameter yang digunakan adalah minimum support 5 persen, minimum confidence 50 persen, minimum lift 1, dan maximum panjang itemset 3.

Apriori digunakan untuk mencari frequent itemsets berdasarkan minimum support. Setelah frequent itemsets ditemukan, association rules dibuat berdasarkan minimum confidence. Rules kemudian difilter berdasarkan lift minimal 1 agar hanya hubungan positif yang ditampilkan.

FP-Growth juga digunakan untuk mencari frequent itemsets dan association rules. FP-Growth biasanya lebih cepat dibandingkan Apriori karena menggunakan struktur FP-Tree dan tidak perlu membentuk kandidat itemset sebanyak Apriori.

Walaupun Association Rule Mining bukan supervised learning, saya tetap membagi data menjadi training dan testing untuk memenuhi ketentuan tugas. Data training digunakan untuk membentuk rules, sedangkan data testing digunakan untuk mengecek apakah rules tersebut masih relevan.

Pada tahap evaluasi, metrik yang digunakan adalah support, confidence, lift, leverage, conviction, jumlah frequent itemsets, dan jumlah association rules. Support menunjukkan seberapa sering itemset muncul. Confidence menunjukkan tingkat kepercayaan sebuah aturan. Lift menunjukkan kekuatan hubungan antar item.

Karena metode asosiasi tidak memiliki akurasi seperti klasifikasi, maka kriteria sukses 80 persen diukur dari rules dengan confidence minimal 80 persen, rata-rata confidence rules terbaik minimal 80 persen, atau test confidence pada data testing minimal 80 persen.

Saya juga membuat visualisasi berupa bar chart item paling sering muncul, scatter plot support vs confidence dengan lift sebagai warna, histogram support-confidence-lift, serta heatmap co-occurrence item. Visualisasi ini membantu memahami hasil analisis dengan lebih mudah.

Tahap terakhir adalah deployment. Hasil project ini dapat dipublikasikan dalam bentuk Google Sites sebagai website portofolio. Isi Google Sites meliputi judul project, identitas mahasiswa, deskripsi studi kasus, dataset, tahapan CRISP-DM, visualisasi hasil, screenshot coding, rules terbaik, kesimpulan, link GitHub, dan link YouTube presentasi.

Kesimpulan dari project ini adalah dataset respons pelanggan cafe terhadap promo digital dapat dianalisis menggunakan Association Rule Mining karena memiliki format transaksi melalui kolom association_items. Algoritma Apriori dan FP-Growth dapat digunakan untuk menemukan frequent itemsets dan association rules.

Rules terbaik dapat digunakan sebagai dasar rekomendasi strategi promosi digital. Jika suatu rules memiliki confidence tinggi dan lift lebih dari 1, maka hubungan antar item dalam rules tersebut dapat dianggap positif dan layak dijadikan bahan pertimbangan dalam pengambilan keputusan.

Sekian presentasi saya mengenai project UAS Data Mining dengan metode Association Rule Mining. Terima kasih. Wassalamualaikum warahmatullahi wabarakatuh.
