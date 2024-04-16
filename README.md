# 2108107010024_Pertemuan_11_ANN


Nama: Ulan Sawalia

NPM : 2108107010024

Materi bacaan:

https://www.megabagus.id/deep-learning-artificial-neural-networks/ (halaman 1 - 7)
⁠⁠https://www.megabagus.id/deep-learning-artificial-neural-networks-aplikasi (halaman 1 - 4)
Pahami isi dari kedua artikel tersebut dan kerjakan:

Contoh pada artikel kedua menggunakan tensorflow pada python environment
⁠Tugas 2 sebelumnya menggunakan SVM, kerjakan dengan menggunakan ANN pada python environment yang sama
Kumpulkan kedua tugas tersebut menggunakan repository pada github dengan nama repository: NPM_Pertemuan_11_ANN. Repository tersebut berisi:

Dataset sebelum dipreprocessing (format csv)
⁠Kode python yang memuat process preprocessing, training, testing dan perhitungan akurasi
⁠File requirements.txt yang berisi library yang digunakan
⁠File README.md yang berisi penjelasan tentang kedua tugas yang dikerjakan beserta perbandingan akurasi SVM dan ANN

dataset yang dipakai:

kalsifikasi


Dataset

dataset yang saya ambil berasal dari Kaggle: https://www.kaggle.com/datasets/yasserh/heart-disease-dataset/data 

dataset ini memprediksi penyakit jantung dengan 14 atribut

*Informasi Atribut: 
1. age	(umur dalam tahun)
2. sex  ((1 = laki-laki; 0 = perempuan))
3. cp (tipe nyeri dada)
   * 0 : Angina tipikal: nyeri dada berhubungan dengan penurunan suplai darah ke jantung
   * 1 : Angina atipikal: nyeri dada yang tidak berhubungan dengan jantung
   * 2 : Nyeri non-angina: biasanya kejang esofagus (tidak berhubungan dengan jantung)
   * 3 : Tanpa gejala : nyeri dada tidak menunjukkan tanda-tanda penyakit
4. trestbps (tekanan darah istirahat (dalam mm Hg saat masuk rumah sakit) - angka di atas 130-140 biasanya menimbulkan kekhawatiran)
5. chol (kolesterol serum dalam mg/dl - serum = LDL + HDL + 0,2 * trigliserida - di atas 200 patut dikhawatirkan)
6. fbs ((gula darah puasa > 120 mg/dl) (1 = benar; 0 = salah) - '>126' mg/dL menandakan diabetes)
7. restecg (hasil elektrokardiografi istirahat)
   * 0 : Tidak ada yang perlu diperhatikan
   * 1 : Kelainan Gelombang ST-T - dapat berkisar dari gejala ringan hingga masalah parah - menandakan detak jantung tidak normal
   * 2 : Kemungkinan atau pasti hipertrofi ventrikel kiri - Pembesaran ruang pompa utama jantung

8. thalach	(detak jantung maksimum tercapai)
9. exang (angina akibat olahraga (1 = ya; 0 = tidak))
10. oldpeak (Depresi ST yang disebabkan oleh olahraga dibandingkan dengan istirahat - melihat stres jantung saat berolahraga - jantung yang tidak sehat akan lebih stres)
11. slope (kemiringan puncak latihan segmen ST)
     * 0 : Menanjak: detak jantung lebih baik dengan olahraga (jarang)
     * 1 : Miring datar: perubahan minimal (tipikal jantung sehat)
     * 2 : Menurun: tanda-tanda jantung tidak sehat
12. ca	(ngiografi koroner - jumlah pembuluh darah besar (0-3) yang diwarnai dengan fluoroskopi - pembuluh darah berwarna berarti dokter dapat melihat darah yang melewatinya - semakin banyak pergerakan darah semakin baik (tidak ada gumpalan))
13. thal (hasil stres talium)
14. target (menderita penyakit atau tidak (1=ya, 0=tidak) (= atribut yang diprediksi))

Studi Kasus : Memprediksi penyebab penyakit jantung


regresi

Dataset

dataset yang saya ambil berasal dari Kaggle: https://www.kaggle.com/datasets/neuromusic/avocado-prices

Dataset yang berisi kumpulan data yang berisi informasi tentang harga dan penjualan avokad dari berbagai wilayah di Amerika Serikat.

*Informasi Atribut: 
1. Date 
2. AveragePrice 
3. type 
4. year 
5. Region 
6. Total volume
7. 4046 - total buah terjual 4046
8. 4225 - total buah terjual 4225
9. 4770 - total buah terjual 4770
10. Total Bags	
11. Small Bags	
12. Large Bags	
13. XLarge Bags

Studi Kasus : Memprediksi harga dari buah alpukat di wilayah Amerika Serikat


## Perbandingan hasil SVM dan ANN

## Klasifikasi
1. SVM model dengan kernel RBF berhasil memprediksi dengan akurasi 70%
2. ANN berhasil memprediksi nilai akurasi 80.33%

## Regresi
1. SVM model dengan polynomial derajat 3 memperoleh nilaiMean Squared Error (MSE): 0.09633212179458203
2. ANN model  menggunakan loss mendapat nilai Loss:  [-189480128.0, 0.0084931505843997]
