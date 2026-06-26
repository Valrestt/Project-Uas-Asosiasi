# Analisis Pola Asosiasi Respons Pelanggan Cafe terhadap Promo Digital

## Deskripsi Project
Project ini merupakan tugas UAS Data Mining dengan metode Association Rule Mining. Dataset yang digunakan adalah Dataset Respons Pelanggan Cafe terhadap Promo Digital. Analisis dilakukan menggunakan framework CRISP-DM dan algoritma Apriori serta FP-Growth.

## Tujuan Project
- Menemukan pola asosiasi antar atribut pelanggan, jenis promo, channel promo, dan event respons pelanggan.
- Membandingkan hasil algoritma Apriori dan FP-Growth.
- Mengevaluasi rules menggunakan support, confidence, lift, leverage, dan conviction.
- Menentukan apakah rules memenuhi kriteria sukses confidence minimal 80%.

## Dataset
Dataset berisi kolom `customer_id`, `gender`, `age_group`, `income_group`, `offer_id`, `offer_type`, `difficulty_group`, `reward_group`, `duration_group`, `channel_web`, `channel_email`, `channel_mobile`, `channel_social`, `event`, dan `association_items`.

## Framework CRISP-DM
1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Modeling
5. Evaluation
6. Deployment

## Algoritma
- Apriori
- FP-Growth

## Library
- pandas
- numpy
- matplotlib
- seaborn
- mlxtend
- scikit-learn

## Cara Menjalankan
1. Pastikan file dataset CSV berada dalam folder yang sama dengan notebook.
2. Install library yang dibutuhkan:
   ```bash
   pip install pandas numpy matplotlib seaborn mlxtend scikit-learn
   ```
3. Jalankan notebook `.ipynb` menggunakan Jupyter Notebook atau Google Colab.

## Output Analisis
- Frequent itemsets Apriori dan FP-Growth
- Association rules Apriori dan FP-Growth
- Evaluasi support, confidence, lift, leverage, conviction
- Evaluasi kriteria sukses 80%
- Visualisasi hasil analisis
- Template deployment Google Sites

## Link Portofolio
- Google Sites: [Masukkan link Google Sites]
- YouTube Presentasi: [Masukkan link YouTube]
