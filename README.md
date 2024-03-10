Foto - Foto ScreenShot:

1. Foto Jmeter sebelum Optimize


All Student
[Image1](test_plan_1.png)

All Student Name
[Image2](test_plan_2.png)

Highest GPA
[Image3](test_plan_3.png)

2. Foto Log sebelum Optimize

All Student
[Image4](testresult1.png)

All Student Name
[Image5](testresult2.png)

Highest GPA
[Image6](testresult3.png)

3. Foto Jmeter Sesudah Optimize
   
All Student
[Image7](test_plan_4.png)

All Student Name
[Image8](test_plan_5.png)

Highest GPA
[Image9](test_plan_6.png)

4. Foto Log Sesudah Optimize

All Student
[Image10](testresult4.png)

All Student Name
[Image11](testresult5.png)

Highest GPA
[Image12](testresult6.png)


REFLEKSI:

Kesimpulan :

Dari perbandingan Pada test_plan Jmeter sebelum dan sesudah optimisasi,
Pada kasus method all-student-request dari profiling yang ada di intelij sebelum optimisasi sekitar 8500 ms dan sesudah optimisasi beredar di antara 1500 ms
dan Jmeternya sample timenya berubah dari sebelumnya 178000 ms ke 3800 ms. Ini menunjukan kenaikan sekitar 96% pada performancenya.

Lalu selanjutnya pada kasus method all-student-name di Pada profiling dari 430 ms ke 320 ms pada Jmeter berubah dari 2300 ms ke sekitar 90 ms, yang
menunjukkan kenaikan performance sebesar lebih dari 80%

Lalu selanjutnya pada kasus method highest gpa di Pada profiling dari 800 ms ke 300 ms pada Jmeter berubah dari 500 ms ke sekitar 150 ms, yang
menunjukkan kenaikan performance sebesar lebih dari 80%

Sehingga dari pengukuran Jmeter diketahui bahwa performance nya naik besar setelah dilakukan optimisasi. Kita memakai jmeter karena lebih konsisten daripada beberapa kasus di profiling java.


1. What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?

Pendekatan uji kinerja pakai JMeter dan pemetaan pakai Profiler IntelliJ beda dalam mengasah performa aplikasi. JMeter dipake buat uji beban, stres, dan performa aplikasi dengan bikin simulasi beban berat di server, jaringan, atau objek buat analisis performa sistem secara keseluruhan di berbagai situasi. Sementara, Profiler IntelliJ dipake buat memetakan aplikasi Java lebih detail, ngeidentifikasi masalah performa dalam kode aplikasi, kayak penggunaan CPU, memori, aktivitas thread, dan hotspot metode.

Pake JMeter, fokusnya lebih ke ngerti gimana aplikasi ngelakuin performa di bawah berbagai beban, sambil cari titik-titik bottlenecks performa. Sementara, pake Profiler IntelliJ lebih ke ngerti gimana aplikasi kerja di dalamnya, ngeidentifikasi jalur kode atau metode tertentu yang bikin masalah performa. Keduanya penting buat optimasi performa aplikasi secara keseluruhan.

2. How does the profiling process help you in identifying and understanding the weak points in your application?

Proses pemetaan membantu kita menemukan di mana aplikasi kita mungkin bermasalah dan bagaimana aplikasi itu bekerja saat dijalankan. Misalnya, dengan melihat berapa banyak CPU atau memori yang digunakan oleh aplikasi, kita bisa tahu apakah ada bagian dari kode yang memakan banyak sumber daya. Selain itu, kita bisa melihat bagaimana thread (urutan tugas) dalam aplikasi bekerja, apakah ada yang terjebak (deadlock) atau terlalu banyak bersaing satu sama lain.

Pemetaan juga membantu kita melihat bagian mana dari aplikasi yang sering dipanggil atau dieksekusi, yang mungkin memerlukan perbaikan. Jika ada metode atau bagian kode tertentu yang memakan waktu eksekusi yang lama, kita bisa fokus untuk memperbaikinya agar aplikasi menjadi lebih cepat dan responsif. Dengan memahami cara kerja aplikasi kita secara detail menggunakan pemetaan, kita dapat membuatnya lebih efisien dan lebih baik dalam menjalankan tugas-tugasnya.

3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?

Menurut saya iya karena  Profiler IntelliJ terbukti efektif dalam membantu pengembang menganalisis dan mengidentifikasi bottleneck dalam kode aplikasi mereka. Dengan menyediakan data lengkap tentang penggunaan CPU, alokasi memori, aktivitas thread, dan waktu eksekusi metode, Profiler IntelliJ memungkinkan pengembang untuk dengan akurat mengidentifikasi area kode yang mungkin menyebabkan penurunan kinerja. Selain itu, alat visualisasi dan laporan detail yang disediakan oleh Profiler IntelliJ memudahkan pengembang untuk memahami dan menginterpretasikan data pemetaan, sehingga mereka dapat dengan cepat mengidentifikasi hotspot dan area yang perlu dioptimalkan dalam kode mereka.

Dengan fitur-fitur yang kuat dan antarmuka yang intuitif, Profiler IntelliJ adalah alat yang berharga bagi pengembang yang ingin meningkatkan kinerja aplikasi Java mereka. Kemampuannya untuk menyediakan wawasan mendalam tentang perilaku runtime aplikasi memungkinkan pengembang untuk mengatasi bottleneck kinerja dan meningkatkan kualitas aplikasi mereka dengan lebih efektif.

4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?

Menurut saya yang susah adalah ketika membuat method-method yang lebih efektif dari method-method lama. Sehingga performance kode yang dimiliki bisa meningkat drastis dari sebelumnya.

5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?


Menggunakan Profiler IntelliJ untuk memeriksa kode aplikasi membawa manfaat besar bagi saya dengan contoh sebagai berikut. Pertama, Profiler memberikan informasi lengkap tentang kinerja aplikasi seperti penggunaan CPU, alokasi memori, aktivitas thread, dan waktu eksekusi metode. Dengan informasi ini, pengembang bisa lebih paham tentang bagaimana aplikasi mereka bekerja dan fokus untuk membuatnya lebih baik. Selain itu, Profiler membantu mengidentifikasi bagian kode yang menyebabkan kinerja aplikasi melambat, sehingga pengembang bisa fokus memperbaikinya.

Profiler IntelliJ juga menyediakan grafik dan laporan yang mudah dimengerti, sehingga pengembang bisa lebih cepat mengerti data yang mereka peroleh. Dengan bantuan visualisasi ini, pengembang bisa melihat di mana masalah kinerja terjadi dan bagaimana memperbaikinya. Selain itu, karena terintegrasi dengan IntelliJ IDEA, Profiler memudahkan pengembang untuk menggunakan alat ini langsung dari lingkungan pengembangan yang mereka kenal. Hal ini membuat proses pemantauan dan perbaikan kinerja aplikasi menjadi lebih efisien dan lancar.

6. How do you handle situations where the results from profiling with Inte	lliJ Profiler are not entirely consistent with findings from performance testing using JMeter?

Ketika hasil dari pemetaan dengan Profiler IntelliJ dan pengujian kinerja menggunakan JMeter tidak sama, penting untuk menangani masalahnya secara teratur. Pastikan kondisi uji yang sama, cek perangkat keras, pengaturan perangkat lunak, jaringan, dan data uji. Ketahui perbedaan metode: pemetaan melihat cara aplikasi bekerja dan masalah pada kode, JMeter menguji kinerja sistem di bawah beban. Meskipun beda, cari kesamaan antara keduanya karena bisa memberikan petunjuk tentang masalah kinerja.

Jika masi agak tidak konsisten bisa ditest beberapa kali hingga konsisten. Apabila masi salah maka saya akan mengambil hasi dari Jmeter karena menurut saya Jmeter lebih konsisten dibanding Profiling intelij

7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?

Saya menggunakan strategi pemanfaatan query dari library JPArepository cth SELECT .. Fetch .. untuk mengoptimisasinya. Dengan melakukan query langsung maka saya tidak perlu menjalankan loop tidak berguna
yang ada pada kode sebelumnya yang hanya membuang buang waktu saja. Dengan menggunakan algo terbaru tanpa loop maka performance naik 80% keatas semua untuk semua method yang ada.

Untuk memastikan bahwa hasilnya benar adalah dengan membandingkan hasil sebelum optimisasi dan sesudah. Langsung tembek request ke url dan liat hasilnya. Setelah diliat hasilnya sama sesuai dengan keinginan maka pasti 
method yang sesudah optimisasi pasti benar dengan sebelum optimisasi.