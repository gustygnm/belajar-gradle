## Belajar Gradle
### Pekerjaan rumah 16 | Module 18 | Profession QA Engineer | Jayjay

Tugas khusus Gradle dan add libraries

Kriteria:
- Buat tugas Gradle sederhana untuk menerima parameter CLI dan mencetaknya dengan pesan ucapan
- Proyek skrip Gradle harus dibuat di repositori yang berbeda dan dorong ke GitHub

### Berikut adalah langkah-langkah untuk membuat tugas khusus Gradle dan menambahkan pustaka:
1. Buat proyek Gradle baru dengan menjalankan perintah "gradle init --type java-library". Ini akan membuat proyek Gradle baru dengan struktur direktori dan file build.gradle awal.
2. Buka file build.gradle di direktori root proyek dan tambahkan kode berikut untuk menentukan tugas khusus:

```
   tasks.register('greetingTask') {
    doLast {
        String nama = project.hasProperty('nama') ? project.property('nama') : 'Gradle User'
        println "Hello, $nama! Welcome to Gradle World!"
    }
   }
```

### Untuk menjalankan tugas gunakan perintah berikut: 
```
./gradlew greetingTask -Pnama=YourName"

```

### Hasil menjalankan perintah:
![Image](https://github.com/gustygnm/belajar-gradle/blob/master/Screenshot%202024-08-14%20at%2011.30.52.png)
