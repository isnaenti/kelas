# ANN
Kerjakan:
1. Jelaskan beberapa contoh fungsi aktivasi
   Fungsi aktivasi dalam ANN digunakan untuk memperkenalkan non-linearitas ke dalam model, memungkinkan jaringan untuk belajar dan memodelkan data yang kompleks.
   contoh fingsi aktivasi :
   a) Sigmoid (logistic) Function:
      Fungsi aktivasi sigmoid, juga dikenal sebagai fungsi aktivasi logistik, mengambil masukan dan mengubahnya menjadi keluaran yang berkisar antara 0 dan 1. Ini sangat berguna untuk tugas klasifikasi atau prediksi probabilitas sehingga dapat diimplementasikan ke dalam pelatihan visi komputer dan jaringan pembelajaran mendalam.
![image](https://github.com/isnaenti/kelas/assets/100338225/0345a767-d5e3-4f69-bb9e-12347c8c01a3)
![image](https://github.com/isnaenti/kelas/assets/100338225/ffa23ca8-e913-4b04-85ab-9db19a3104e8)

   b) Tanh (Hyperbolic Target) Function:
      Tanh (atau TanH), juga dikenal sebagai fungsi aktivasi tangen hiperbolik, mirip dengan sigmoid/logistik, bahkan hingga kurva bentuk S, dan dapat dibedakan. Kecuali, dalam kasus ini, rentang keluarannya adalah -1 hingga 1 (bukan 0 hingga 1). Karena keluaran tanh bersifat zero-centric, nilainya dapat lebih mudah dipetakan pada skala antara sangat negatif, netral, atau positif.

  ![image](https://github.com/isnaenti/kelas/assets/100338225/b66cc3f4-93d4-4bf3-af46-84b75ccd2159)
  
    
   c) ReLU (Rectified Linear Unit) Function:
       ReLU memiliki fungsi turunan dan memungkinkan propagasi mundur sekaligus membuatnya efisien secara komputasi. Masalah utama di sini adalah fungsi ReLU tidak mengaktifkan semua neuron secara bersamaan. Neuron hanya akan dinonaktifkan jika keluaran transformasi linier kurang dari 0.

![image](https://github.com/isnaenti/kelas/assets/100338225/ddecaa79-bf15-4e3a-b2a2-c8a94bd2ea7d)
Keunggulan Leaky ReLU sama dengan ReLU, selain memungkinkan propagasi mundur, bahkan untuk nilai input negatif. Dengan melakukan sedikit modifikasi pada nilai masukan negatif, gradien sisi kiri grafik menjadi nilai bukan nol. Oleh karena itu, kita tidak akan lagi menemukan neuron mati di wilayah tersebut. 

   d) Leacky ReLU Function
      Leaky ReLU merupakan versi perbaikan dari fungsi ReLU untuk mengatasi masalah Dying ReLU karena memiliki kemiringan positif yang kecil di area negatif.
![image](https://github.com/isnaenti/kelas/assets/100338225/370c181b-cb33-4554-8240-3160216323b4)

   e) Softmax Function
       Fungsi Softmax digambarkan sebagai kombinasi beberapa sigmoid. Ini menghitung probabilitas relatif. Mirip dengan fungsi aktivasi sigmoid/logistik, fungsi SoftMax mengembalikan probabilitas setiap kelas. Ini paling sering digunakan sebagai fungsi aktivasi untuk lapisan terakhir jaringan saraf dalam kasus klasifikasi kelas jamak.
![image](https://github.com/isnaenti/kelas/assets/100338225/037ed889-32a5-4a2b-a8b2-22e1fdd10d2b)


   f) Swish Function
       Swish secara konsisten mencocokkan atau mengungguli fungsi aktivasi ReLU pada jaringan dalam yang diterapkan pada berbagai domain menantang seperti klasifikasi gambar , terjemahan mesin, dll.
![image](https://github.com/isnaenti/kelas/assets/100338225/2c268c86-77b8-4d93-abcf-a0c7e417e6ed)

3. Coba gambarkan dan jelaskan beberapa arsitektur berikut:
   * GAN
   * AE
   * LSTM
   * VGG
   * RNN
4. Buatkan kodingan from scracth NN
