# Sistem Pendeteksi Penyakit Kardiovaskular Berbasis Teks


## Deskripsi Singkat
Sistem ini adalah implementasi deteksi penyakit kardiovaskular berbasis teks yang menggunakan model BERT (Bidirectional Encoder Representations from Transformers) untuk menganalisis teks keluhan pasien dan memberikan prediksi apakah pasien mungkin mengidap penyakit kardiovaskular atau tidak.

## Fitur Utama
Analisis keluhan pasien berdasarkan model BERT.
Pemahaman konteks kata untuk interpretasi keluhan secara menyeluruh.
Fine-tuning untuk meningkatkan kinerja pada dataset kesehatan spesifik.

## Atribut Dataset
1. "Keluhan": teks keluhan pasien
2. "Kardiovaskuler": "0" apabila keluhan bukan penyakit kardiovaskuler dan "1" apabila keluhan merupakan penyakit kardiovaskuler
(kolom "Clean_Keluhan" ditambahkan untuk menyimpan hasil pembersihan teks keluhan)

## Langkah-langkah menjalankan program
1. Unduh dataset "dataset_v1.0.xlsx"
2. Simpan dataset di Google Drive Anda
3. Buka file "cardiovascular_detection.ipynb" lalu jalankan program (disarankan menggunakan https://colab.research.google.com/)
4. ![image](https://github.com/aureliasknt/cardiovascular_detection/assets/100254279/62367f0e-05bb-4047-914e-82be454e3b74)
Ganti bagian "/content/drive/MyDrive/omnifit/dataset" dengan path yang sesuai dengan posisi dataset dalam GDrive Anda
5. ![image](https://github.com/aureliasknt/cardiovascular_detection/assets/100254279/324e2a1c-37a9-4c5a-94c2-bc37e4f1cc88)
Klik "Run all" untuk menjalankan program
6. Skor Accuracy dan Loss dapat dilihat di bagian "8. Model Evaluation"
7. ![image](https://github.com/aureliasknt/cardiovascular_detection/assets/100254279/1f8a14f0-2573-4a46-9e46-5ab35677e3ad)
Pada bagian tersebut Anda bisa menginputkan teks keluhan pasien untuk diprediksi.
Sebagai referensi, berikut merupakan teks keluhan pasien yang diambil dari situs alodokter.com "https://www.alodokter.com/komunitas/topic/penyebab-rasa-sakit-di-dada-kiri-seperti-ditusuk-jarum":
"Siang dokter, izin bertanya. Tadi ayah saya cerita, kalo sudah beberapa kali di dadanya yg sebelah kiri muncul rasa sakit yg tiba". Rasa sakit yg beliau bilang itu kaya kalo dada kita ditusuk" pake jarum, ayah saya sata ini umurnya 56 tahun dok, kira" penyebab rasa sakit yg ayah saya alami ini apa ya dok?"
8. Output hasil prediksi dapat dilihat di bagian paling akhir program:
![image](https://github.com/aureliasknt/cardiovascular_detection/assets/100254279/dd27a438-83d5-42ee-9652-8f76e944c3b4)
