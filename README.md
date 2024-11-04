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
