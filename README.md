# Exercise-Profiling  
### Fikri Dhiya Ramadhana  
### 2206819533
### Advanced Programming - C

1. Screenshots JMeter GUI (unoptimized)
    * Test Plan 1 (all-student)
   ![test_plan_1.png](images%2Ftest_plan_1.png)
    * Test Plan 2 (all-student name)
   ![test_plan_2.png](images%2Ftest_plan_2.png)
    * Test Plan 3 (highest-gpa)
   ![test_plan_3.png](images%2Ftest_plan_3.png)
   
2. Screenshots JMeter Log (unoptimized)
    * Test Result Log 1 (all-student)
   ![test_result_log_1.png](images%2Ftest_result_log_1.png)
    * Test Result Log 2 (all-student name)
   ![test_result_log_2.png](images%2Ftest_result_log_2.png)
    * Test Result Log 3 (highest-gpa)
   ![test_result_log_3.png](images%2Ftest_result_log_3.png)

3. Screenshots JMeter GUI (optimized)
   * Test Plan 1 (all-student)
     ![Screenshot 2024-03-13 at 19.44.09.png](images%2FScreenshot%202024-03-13%20at%2019.44.09.png)
   * Test Plan 2 (all-student name)
     ![Screenshot 2024-03-13 at 19.46.05.png](images%2FScreenshot%202024-03-13%20at%2019.46.05.png)
   * Test Plan 3 (highest-gpa)
     ![Screenshot 2024-03-13 at 19.47.16.png](images%2FScreenshot%202024-03-13%20at%2019.47.16.png)

4. Screenshots JMeter Log (optimized)
   * Test Result Log 1 (all-student)
     ![Screenshot 2024-03-13 at 19.45.20.png](images%2FScreenshot%202024-03-13%20at%2019.45.20.png)
   * Test Result Log 2 (all-student name)
     ![Screenshot 2024-03-13 at 19.46.42.png](images%2FScreenshot%202024-03-13%20at%2019.46.42.png)
   * Test Result Log 3 (highest-gpa)
     ![Screenshot 2024-03-13 at 19.47.47.png](images%2FScreenshot%202024-03-13%20at%2019.47.47.png)

## Reflection

1. What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?  
perbedaan antara JMeter dengan InteliJ Profiler:  
   * JMeter: memiliki fokus dalam response time, throughtput dan scalability dari aplikasi dengan generating load untuk mengidentifikasi suatu bottleneck kinerja.
   * IntelliJ Profiler: memiliki fokus dalam mengidentifikasi kebocoran memori, CPU loads, dan alokasi objek dengan menemukan area kode yang spesifik untuk di optimisasi.  
  

2. How does the profiling process help you in identifying and understanding the weak points in your application?  
Dengan melihat flametree, list method, dan timeline yang digunakan dari kode yang dijalankan.  
  

3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?  
Menurut saya, IntelliJ Profiler merupakan solusi terbaik untuk melihat complexity dari setiap kode method yang kita buat karena dapat memberikan keterangan mengenai CPU Time dari method yang dipanggil.  
  

4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?  
Mungkin tantangan yang saya rasakan adalah beradaptasi dengan enviroment baru karena profiling baru pertama kali saya lakukan di IDE ini karena sebelumnya saya selalu menggunakan VSCode. Cara saya untuk menaklukan tantangan tersebut adalah mencari dokumentasi bagaimana cara menggunakan IntelliJ Idea Ultimate ini agar bisa menggunakannya dengan optimal.  
  

5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?  
Mudah untuk mencari method yang masih dapat dioptimisasikan karena semuanya dapat terlihat di flametree secara detail.  
  

6. How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?  
Hal ini dapat ditangani dengan melakukan cross-verification antara kedua result untuk melihat perbedaan agar dapat dianalisis kekonsistenannya.  
  

7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?  
Strategi yang dapat dilakukan adalah membuat database dengan data yang banyak, lalu dilakukannya profiling terhadap endpoint - endpoint yang ada sehingga dapat dilihat perbedaan dari bagian kode yang sudah teroptimisasi dan yang masih bisa dioptimisasikan lagi. Contohnya seperti pada exercise ini adalah menghilangkan nested loop agar kompleksitasnya lebih kecil dan penggunaan StringBuilder untuk meningkatkan performa. Dan perlu dilakukan unit dan functional tests ulang agar kita bisa mengetahui bahwa fungsionalitas dari aplikasi yang dibuat tidak berubah.
