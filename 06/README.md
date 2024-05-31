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
   
![image](https://github.com/isnaenti/kelas/assets/100338225/9f569a48-a9e1-49ec-882a-264f7e73a707)
![image](https://github.com/isnaenti/kelas/assets/100338225/b66cc3f4-93d4-4bf3-af46-84b75ccd2159)
  
    
   c) ReLU (Rectified Linear Unit) Function:

   ReLU memiliki fungsi turunan dan memungkinkan propagasi mundur sekaligus membuatnya efisien secara komputasi. Masalah utama di sini adalah fungsi ReLU tidak mengaktifkan semua neuron secara bersamaan. Neuron hanya akan dinonaktifkan jika keluaran transformasi linier kurang dari 0.Keunggulan Leaky ReLU sama dengan ReLU, selain memungkinkan propagasi mundur, bahkan untuk nilai input negatif. Dengan melakukan sedikit modifikasi pada nilai masukan negatif, gradien sisi kiri grafik menjadi nilai bukan nol. Oleh karena itu, kita tidak akan lagi menemukan neuron mati di wilayah tersebut. 
   
![image](https://github.com/isnaenti/kelas/assets/100338225/173345e5-dccf-4510-98e0-572341dc227e)

![image](https://github.com/isnaenti/kelas/assets/100338225/ddecaa79-bf15-4e3a-b2a2-c8a94bd2ea7d)


   d) Leacky ReLU Function
      
   Leaky ReLU merupakan versi perbaikan dari fungsi ReLU untuk mengatasi masalah Dying ReLU karena memiliki kemiringan positif yang kecil di area negatif.Keunggulan Leaky ReLU sama dengan ReLU, selain memungkinkan propagasi mundur, bahkan untuk nilai input negatif. Dengan melakukan sedikit modifikasi pada nilai masukan negatif, gradien sisi kiri grafik menjadi nilai bukan nol. Oleh karena itu, kita tidak akan lagi menemukan neuron mati di wilayah tersebut. 

![image](https://github.com/isnaenti/kelas/assets/100338225/21e3915a-5461-42e8-a0ad-9b7423a78314)
![image](https://github.com/isnaenti/kelas/assets/100338225/370c181b-cb33-4554-8240-3160216323b4)

   e) Softmax Function
      
   Fungsi Softmax digambarkan sebagai kombinasi beberapa sigmoid. Ini menghitung probabilitas relatif. Mirip dengan fungsi aktivasi sigmoid/logistik, fungsi SoftMax mengembalikan probabilitas setiap kelas. Ini paling sering digunakan sebagai fungsi aktivasi untuk lapisan terakhir jaringan saraf dalam kasus klasifikasi kelas jamak. Fungsi ini mengembalikan 1 untuk indeks probabilitas terbesar sementara mengembalikan 0 untuk dua indeks array lainnya. Di sini, memberikan bobot penuh pada indeks 0 dan tidak ada bobot pada indeks 1 dan indeks 2. Jadi outputnya adalah kelas yang sesuai dengan neuron pertama (indeks 0) dari tiga.

![image](https://github.com/isnaenti/kelas/assets/100338225/e6812519-5509-427d-a9be-f9589ba39b3b)
![image](https://github.com/isnaenti/kelas/assets/100338225/037ed889-32a5-4a2b-a8b2-22e1fdd10d2b)


   f) Swish Function
       
   Swish secara konsisten mencocokkan atau mengungguli fungsi aktivasi ReLU pada jaringan dalam yang diterapkan pada berbagai domain menantang seperti klasifikasi gambar , terjemahan mesin, dll. keunggulan fungsi aktivasi Swish dibandingkan ReLU: fSwish adalah fungsi halus yang artinya tidak berubah arah secara tiba-tiba seperti yang dilakukan ReLU di dekat x = 0. Sebaliknya, fungsi tersebut secara mulus membengkok dari 0 menuju nilai < 0 dan kemudian naik lagi.
      
![image](https://github.com/isnaenti/kelas/assets/100338225/2c268c86-77b8-4d93-abcf-a0c7e417e6ed)

2. Coba gambarkan dan jelaskan beberapa arsitektur berikut:
   * GAN
   Jaringan adversarial generatif (GAN) adalah sebuah arsitektur deep learning. Arsitektur ini melatih dua jaringan neural untuk saling bersaing agar dapat menghasilkan data baru yang lebih autentik dari set data pelatihan yang diberikan. Misalnya, Anda dapat menghasilkan gambar baru dari basis data gambar yang ada atau musik asli dari basis data lagu. GAN disebut adversarial karena melatih dua jaringan yang berbeda dan mengadu keduanya. Jaringan pertama menghasilkan data baru dengan mengambil sampel data input dan memodifikasinya semaksimal mungkin.

![image](https://github.com/isnaenti/kelas/assets/100338225/5157e92a-ff9a-4657-8e9c-eee035db17fb)

   * AE
   Autoencoder adalah jenis arsitektur jaringan saraf yang dirancang untuk secara efisien mengompresi (encode) data input hingga ke fitur-fitur esensialnya, kemudian merekonstruksi (decode) input asli dari representasi yang dikompresi ini. Autoencoder merujuk pada subset spesifik arsitektur encoder-decoder yang dilatih melalui pembelajaran yang tidak diawasi untuk merekonstruksi data input sendiri. Karena tidak bergantung pada data pelatihan berlabel, autoencoder tidak dianggap sebagai metode pembelajaran yang diawasi.

Cara kerja autoencoder

Autoencoder menemukan variabel laten dengan melewatkan data input melalui "kemacetan" sebelum mencapai decoder. Hal ini memaksa encoder untuk belajar mengekstrak dan melewatkan hanya informasi yang paling kondusif untuk merekonstruksi input asli secara akurat.

![WhatsApp Image 2024-05-27 at 13 42 42_849f428f](https://github.com/isnaenti/kelas/assets/100338225/84d07f8c-7be4-49d9-bdad-0f991e093e60)

   * LSTM
   LSTM merupakan modifikasi dari RNN yang memiliki memory dan banyak jenis gerbang yaitu input gate, forget gate, dan output gate. LSTM mampu mempelajari lebih dari 1000 langkah sebelumnya tergantung pada kompleksitas jaringan.

![image](https://github.com/isnaenti/kelas/assets/100338225/c9f877c0-18dd-4290-be4a-396d600ce2df)

   * VGG
   VGG ( Grup Geometri Visual ), yang normal dalam Jaringan Saraf Konvolusional ( CNN ) struktur yang terdiri dari beberapa lapisan melahirkan Revolusi Pembelajaran Mendalam yang dipimpin oleh VGG-16 dan VGG-19.

![image](https://github.com/isnaenti/kelas/assets/100338225/1b1dc031-e823-450f-93bb-432606c08087)


Arsitektur VGG

VGGNets didasarkan pada fitur paling penting dari jaringan saraf konvolusional ( CNN ). Grafik berikut menunjukkan konsep dasar tentang cara kerja CNN:

![image](https://github.com/isnaenti/kelas/assets/100338225/0196c6c0-1dc6-404a-aca6-317aa74573b1)

· Input: Ukuran input gambar untuk VGGNet adalah 224 kali 224 piksel. Selain itu, untuk kompetisi ImageNet, pembuat model menghapus patch pusat 224 × 224 di setiap gambar untuk menjaga konsistensi gambar input.
· Lapisan Konvolusional: Lapisan konvolusional VGG menggunakan bidang reseptif minimum 3 × 3 yang kecil, tetapi menggabungkan gerakan naik / turun dan kiri / kanan.
· Lapisan Tersembunyi: Setiap lapisan tersembunyi VGG menggunakan ReLU. Normalisasi Respons Lokal ( LRN ) biasanya tidak dieksploitasi oleh VGG karena menghasilkan memori dan pemborosan waktu pelatihan. Selain itu, tidak meningkatkan akurasi sama sekali.
· Lapisan yang Sepenuhnya Terhubung: Ini, ada tiga lapisan yang sepenuhnya terhubung di VGGnet.

![image](https://github.com/isnaenti/kelas/assets/100338225/adba0723-5b07-495b-9569-d08df85629ea)


   * RNN
(Recurrent Neural Network) adalah salah satu jenis arsitektur ANN yang digunakan untuk memproses data urutan atau rangkaian, seperti teks, audio, atau data waktu. RNN memiliki kemampuan untuk mengingat informasi dari waktu sebelumnya dan menggunakan informasi itu untuk menghasilkan output pada waktu saat ini.

Pada dasarnya, RNN adalah jaringan saraf dengan sambungan siklik, yang memungkinkan informasi untuk disimpan dan diakses dari waktu sebelumnya dalam proses pengolahan. Arsitektur RNN memungkinkan model untuk mengambil keputusan yang lebih cerdas dalam memproses data urutan, karena model dapat mempertimbangkan konteks sebelumnya saat memproses setiap elemen dalam urutan.

![image](https://github.com/isnaenti/kelas/assets/100338225/a126cedc-bd3e-402b-a7c1-0cc7948ba9e6)

3. Buatkan kodingan from scracth NN
```
import numpy as np

# Generate Dummy Data (XOR problem)
X = np.array([[0, 0],
              [0, 1],
              [1, 0],
              [1, 1]])

Y = np.array([[0],
              [1],
              [1],
              [0]])

# Seed the random number generator for reproducibility
np.random.seed(42)

# Initialize weights and biases
input_size = 2  # Number of input features
hidden_size = 2  # Number of neurons in hidden layer
output_size = 1  # Number of output neurons

# Weights for input to hidden layer
W1 = np.random.rand(input_size, hidden_size)
b1 = np.random.rand(hidden_size)

# Weights for hidden to output layer
W2 = np.random.rand(hidden_size, output_size)
b2 = np.random.rand(output_size).reshape(-1)  # Ensure b2 has the shape (1,)

# Define activation functions
def sigmoid(x):
    return 1 / (1 + np.exp(-x))

def sigmoid_derivative(x):
    return x * (1 - x)

# Training parameters
learning_rate = 0.1
epochs = 10000

# Training loop
for epoch in range(epochs):
    # Forward pass
    hidden_input = np.dot(X, W1) + b1
    hidden_output = sigmoid(hidden_input)

    final_input = np.dot(hidden_output, W2) + b2
    final_output = sigmoid(final_input)

    # Calculate the error
    error = Y - final_output
    if (epoch + 1) % 1000 == 0:
        print(f'Epoch {epoch + 1}, Error: {np.mean(np.abs(error))}')

    # Backward pass
    d_output = error * sigmoid_derivative(final_output)
    error_hidden_layer = d_output.dot(W2.T)
    d_hidden_layer = error_hidden_layer * sigmoid_derivative(hidden_output)

    # Update weights and biases
    W2 += hidden_output.T.dot(d_output) * learning_rate
    b2 += np.sum(d_output, axis=0) * learning_rate  # Ensure no keepdims=True

    W1 += X.T.dot(d_hidden_layer) * learning_rate
    b1 += np.sum(d_hidden_layer, axis=0) * learning_rate

# Testing the trained neural network
hidden_input = np.dot(X, W1) + b1
hidden_output = sigmoid(hidden_input)

final_input = np.dot(hidden_output, W2) + b2

final_output = sigmoid(final_input)

print("Predicted Output:")
print(final_output)
```
Hasil dari kodingan diatas outputannya seperti ini:
![image](https://github.com/isnaenti/kelas/assets/100338225/7068d438-661c-4236-af69-dc43ebd17668)

