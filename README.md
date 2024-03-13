# Mahoga Aribowo Heryasa

# 2206025230

<details>
<summary><b><h2>Tutorial 5</h2></b></summary>

## JMeter Table Report dan Test Result

### `/all-student`
 
- JMeter table report (before optimization)

    <img src="src/image/all-student.jpg" alt="all-student JMeter"></img>

- Test result (before optimization)

  <img src="src/image/testresult1.jpg" alt="all-student testresult1.jtl"></img>

- JMeter table report (after optimization)

  <img src="src/image/all-student after.jpg" alt="all-student JMeter optimized"></img>

- salah satu hasil IntelliJ Profiler (execution time)

  | Before Optimization | After Optimization | Performance improvement % |
  |---------------------|--------------------|--------------------------|
  | 5107 ms             | 972 ms             | 80.97%                   |


### `/all-student-name`

- JMeter table report (before optimization)

  <img src="src/image/all-student-name.jpg" alt="all-student-name JMeter"></img>

- Test result (before optimization)

  <img src="src/image/testresult2.jpg" alt="all-student-name testresult2.jtl"></img>

- JMeter table report (after optimization)

  <img src="src/image/all-student-name after.jpg" alt="all-student-name JMeter optimized"></img>

- salah satu hasil IntelliJ Profiler (execution time)

  | Before Optimization | After Optimization | Performance improvement % |
  |---------------------|--------------------|---------------------------|
  | 652 ms              | 122 ms             | 81.29%                    |


### `/higest-gpa`

- JMeter table report (before optimization)

  <img src="src/image/higest-gpa.jpg" alt="higest-gpa JMeter"></img>

- Test result (before optimization)

  <img src="src/image/testresult3.jpg" alt="higest-gpa testresult3.jtl"></img>

- JMeter table report (after optimization)

  <img src="src/image/higest-gpa after.jpg" alt="higest-gpa JMeter optimized"></img>

- salah satu hasil IntelliJ Profiler (execution time)

  | Before Optimization | After Optimization | Performance improvement % |
  |---------------------|--------------------|---------------------------|
  | 121 ms              | 33 ms              | 72.73%                    |

### Conclusion

Berdasarkan perbandingan hasil *sample-time JMeter report* dan perbandingan *execution time IntelliJ Profiler*, terdapat kenaikan performance untuk fungsi-fungsi yang di optimisasi. Hal ini ditandakan dengan *sample-time JMeter* dan *execution time IntelliJ Profiler* yang relatif menurun sehingga program berjalan lebih cepat. Secara keseluruhan, dapat disimpulkan optimisasi yang saya lakukan menghasilkan performance yang relatif lebih baik berdasarkan penggunaan JMeter dan IntelliJ Profiler sebagai alat ukur. 


## Refleksi

### Perbedaan *performance testing* dengan JMeter dan *profiling* dengan IntelliJ Profiler 

Perbedaan *performance testing* dengan JMeter dan *profiling* dengan IntelliJ Profiler dalam konteks optimisasi *performance* adalah JMeter digunakan untuk mengevaluasi respons dan kinerja aplikasi dalam menghadapi beban kerja yang berat atau dalam skenario penggunaan yang tinggi. Sementara IntelliJ Profiler, digunakan untuk menganalisis dan memahami perilaku dan kinerja aplikasi secara detail hingga tingkat kode sehingga mudah untuk mencari titik lemah dan melakukan perbaikan secara langsung.

### Proses *profiling* membantu mengidentifikasi *weak-points*

Proses *profiling* membantu mengidentifikasi dan memahami *weak-points* dalam aplikasi dengan memantau penggunaan sumber daya seperti CPU, memori, dan I/O, melacak waktu eksekusi metode dan fungsi yang memakan waktu yang secara berlebihan, menganalisis alur eksekusi untuk memahami perilaku aplikasi secara keseluruhan, dan mengidentifikasi hotspots atau bagian-bagian kode yang memakan waktu atau sumber daya secara signifikan. Fitur yang tersedia Ini membantu proses optimasi yang tepat untuk meningkatkan kinerja aplikasi.

### efektivitas IntelliJ Profiler

Menurut saya, Intellij Porfiler cukup efektiv dalam membantu mengidentifikasi dan menganalisis *bottlenecks* dalam aplikasi. Terdapat beragam fitur Intellij Profiler yang membantu, seperti *flame graph* yang mempu menunjukkan *hot spot* pada kode aplikasi, *method list tab* yang memapu menunjukkan *execution time* setiap method yang ingin dianalisis, dan *timeline tab* yang mampu menyajikan *timeline* proses aplikasi berjalan secara keseluruhan. 

### Tantangan *profiling* dan *performance testing*

Salah satu tantangan utama yang saya lalui dalam melakukan *profiling* dan *performance testing* adalah memahami data yang disajikan, terutama dalam IntelliJ Profiler, data yang disajikan kurang terasa intuitif sehingga dalam meng-*overcome* tantangan tersebut saya mencoba mencari tau makna dari setiap interpretasi data yang diberikan. Selain itu, tantangan lain yang saya hadapi adalah ketika melakukan optimisasi untuk metode yang memakan waktu yang relatif lama. Dalam proses mencari alogoritma yang lebih efisien, diperlukan ketelitian dan pemahaman yang baik terhadap alur kode.  

### Keuntungan IntelliJ Profiler

Keuntungan utama yang disediakan IntelliJ Profiler adalah menyediakan analisis kinerja lengkap, memudahkan identifikasi titik-titik lemah kinerja, memantau kinerja aplikasi secara real-time, dan intergrasi dengan IntelliJ IDEA yang memudahkan proses analisa karena tidak perlu software atau extension tambahan.

### Inkonsistensi antara IntelliJ Profiler dan JMeter

Berdasarkan hasil temuan yang saya lakukan tidak terdapat inkonsistensi antara hasil IntelliJ Profiler dan JMeter. Namun jika pada kasus lain saya mengalami inkonsitensi, saya akan mencoba melihat konfigurasi *test* dari kedua aplikasi dan merubah konfigurasi jika terdapat konfigurasi yang tidak tepat. jika solusi pertama tidak berhasil, saya akan mencari tahu solusi yang lebih spesifik memalui *internet* atau bertanya kepada asisten dosen.

### Implementasi Optimisasi

Strategi optimisasi

  - Melakukan *profiling* lalu mengidentifikasi metode, fungsi, atau bagian kode yang memiliki *execution time*, *memory allocation*, atau *CPU time* yang tidak efektif.
  - Menganalisis penggunan struktur data dan algoritma yang mungkin kurang tepat sehingga menghasilkan *running time* program yang kurang efisien.
  - Mengurangi penggunaan objek yang tidak diperlukan sehingga menimilkan penempatan memori.
  - Melakukan perubahan pada kode perdasarkan analisis yang telah dilakukan dan menganalisis hasil perubahan optimisasi.

Untuk memastikan perubahan yang dilakukan tidak berdampak pada fungsionalitas aplikasi, dapat kita bandingkan hasil pengambilan data dari setiap fungsi, seperti melihat data hasil pemanggilan `/all-student` sebelum dan sesudah optimisasi. Namun, untuk menjamin kepastian secara menyeluruh dapat dibuat suatu unit test yang memastikan fungsionalitas aplikasi.

</details>