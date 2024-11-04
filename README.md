# Tugas Praktikum 
**NAMA : Alfha Risqi Wicaksono**
**NIM : 362358302145**

Hasil Screenshot Pratikum Pertama:

![Screenshot 2024-11-04 102950](https://github.com/user-attachments/assets/f29a671a-830b-45df-8e75-40b339db6d17)

Hasil Screenshot Pratikum Kedua:

![Screenshot 2024-11-04 105724](https://github.com/user-attachments/assets/3ac5ae04-0964-44ec-bd91-d4ddfe176008)

Hasil Screenshot Pratikum Pertama dan Kedua Setelah digabunggkan:

![Screenshot 2024-11-04 111821](https://github.com/user-attachments/assets/62c73d1a-3423-4114-b8b0-ead7e4e1754c)

Penggambungan dari Pratikum 1 dan 2, merupakan penggabungan kamera dan filter, dari penggabungan pratikum tadi, saya hanya mengubah file main dart. Bagian utama yang menghubungkan kamera dan filter pada kode ini berada di dalam build method dari _CameraWithFilterScreenState, khususnya pada Stack widget yang menyusun layout dari pratinjau kamera dan overlay filter.

```
Positioned(
            bottom: 0,
            left: 0,
            right: 0,
            child: FilterSelector(
              filters: [
                Colors.transparent,
                Colors.red,
                Colors.green,
                Colors.blue,
                Colors.yellow,
              ],
              onFilterChanged: (Color color) {
                setState(() {
                  selectedFilter = color;
                });
```

**Penjelasan Async pada pratikum pertama**

Async digunakan agar fungsi main bisa menjalankan operasi asinkron, memungkinkan penggunaan await untuk menunggu availableCameras() menyelesaikan inisialisasi kamera sebelum melanjutkan ke langkah berikutnya. Dengan Future<void>, fungsi ini tetap tidak mengembalikan nilai spesifik, tetapi tetap menunggu proses asinkron di dalamnya selesai sebelum menjalankan runApp.

**Penjelasan dari anotasi @immutable dan @override**

Dalam Dart, anotasi `@immutable` digunakan untuk menandai bahwa semua properti kelas tidak dapat diubah (immutable) setelah objek dibuat, sehingga setiap properti harus diinisialisasi di konstruktor dan tidak boleh diubah. Ini sering digunakan pada kelas widget di Flutter untuk memastikan konsistensi tampilan. Anotasi `@override`, di sisi lain, digunakan saat sebuah metode pada kelas anak ingin menggantikan implementasi metode yang sama dari kelas induknya. Ini membantu untuk memastikan bahwa metode tersebut benar-benar ada di kelas induk, mengurangi kesalahan ketik dan meningkatkan keterbacaan kode.
