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
</details>