# wireframe
 # Struktur Proyek
 <img width="125" height="103" alt="image" src="https://github.com/user-attachments/assets/c60f1603-9344-416c-bb7e-e047e0eefec6" />
 
 # A. Desain dan konsep layout (wireframe)
 wireframe sederhana yang menampilkan halaman login dan create account
 - Halaman login
   <img width="1919" height="1025" alt="Screenshot 2025-09-15 143457" src="https://github.com/user-attachments/assets/af50fdf9-e418-4c01-bdf8-2b23020bde93" />

 - Halaman pembuatan akun
   <img width="1917" height="1036" alt="Screenshot 2025-09-15 153526" src="https://github.com/user-attachments/assets/a48ceb8e-201d-44b5-8208-43b09d448c19" />


 # B. Latihan untuk Eksplorasi Lebih Lanjut
 Di bagian register
 1.  Validasi Input: Tambahkan validasi yang lebih baik. Misalnya, cek apakah email memiliki format yang benar (mengandung ’@’) atau password memiliki panjang minimal 6 karakter.
    
<img width="431" height="310" alt="image" src="https://github.com/user-attachments/assets/85d859ba-435a-4050-94f7-5ff77df29384" />
    
- validasi email
  disini tidak bisa karena email wajib menggunakan '@' jika tidak menggunakan tanda '@' maka tidak bisa dan akan gagal
  
<img width="959" height="498" alt="image" src="https://github.com/user-attachments/assets/930db035-cdfb-4ec1-8308-a7f3a4b58266" />

- validasi karakter password
  jika karakter passowrdnya kurang dari 6 karakter maka akan menampilkan seperti dibawah
  <img width="723" height="380" alt="image" src="https://github.com/user-attachments/assets/40d5d21f-a1d2-4263-b530-8078727a61f1" />

- berhasil registrasi
  akan menampilkan tulisan berhasil registrasi atau membuat akun 
  <img width="940" height="492" alt="image" src="https://github.com/user-attachments/assets/41a8e257-fbdd-412f-9723-82315c2a1809" />

2. Tampilkan/Sembunyikan Password: Tambahkan ikon mata pada TextField password yang bisa ditekan untuk menampilkan atau menyembunyikan teks password
- register
   
 <img width="440" height="320" alt="image" src="https://github.com/user-attachments/assets/74664f27-57a6-43dd-b721-a4ce9647dfdd" />
 
  tampilan hasil di create account, terdapat ikon mata di password.
  tampilan sebelum penambahan ikon mata di bagian password pembuatan akun
  
  <img width="1917" height="1036" alt="Screenshot 2025-09-15 153526" src="https://github.com/user-attachments/assets/0370f3bf-4a36-44b8-b5bd-182de4e1e543" />

  sesudah penambahan ikon mata dibagian password 
  
 <img width="774" height="408" alt="image" src="https://github.com/user-attachments/assets/151b44ab-c032-428e-9e00-3c65bb98d4af" />

 - login
   
   <img width="376" height="293" alt="image" src="https://github.com/user-attachments/assets/622fa8fe-b3a2-401b-a748-3051426de89a" />

  tampilan hasil di login awal akan muncul ikon mata di bagian pasword.
  tampilan sebelum penambahan ikon mata di password
  
  <img width="1919" height="1025" alt="Screenshot 2025-09-15 143457" src="https://github.com/user-attachments/assets/d0bf132e-323d-4516-a05c-87b0334e2134" />

  tampilan sesudah penambahan ikon mata di password
  
  <img width="742" height="373" alt="image" src="https://github.com/user-attachments/assets/064bbf1b-d514-41d0-8932-61b0c6f3fcf7" />

3. Animasi Sederhana: Tambahkan Hero widget pada ikon di halaman login dan registrasi agar ada transisi animasi yang halus
   - hero di login
     
     <img width="212" height="104" alt="image" src="https://github.com/user-attachments/assets/7b32797c-19ea-4b47-83c9-1b10d2271819" />
     
   - hero di register
     
     <img width="189" height="113" alt="image" src="https://github.com/user-attachments/assets/ede9fc9c-0e5c-4341-b858-b14b6779c36c" />
     
4. Simpan Sesi Login: Coba gunakan package shared_preferences untuk menyimpan status login. Jadi, saat aplikasi ditutup dan dibuka lagi, pengguna tidak perlu login ulang jika sesinya masih aktif.
 - main.dart
   jika user sudah login maka aplikasi langsung buka homepage maka tidak perlu login ulang
   
   <img width="391" height="363" alt="image" src="https://github.com/user-attachments/assets/a49b0988-624a-4542-afaf-7e544397f46c" />

 - homepage
   digunakan untuk  Saat login data sesi disimpan ke SharedPreferences. dan saat aplikasi dibuka ulang  dan data dicek, kalau masih ada berarti user langsung masuk (tidak perlu login lagi).
   
  <img width="337" height="110" alt="image" src="https://github.com/user-attachments/assets/cb64f7d5-fe82-46a2-952e-dd2bf6eb8613" />

  - login
    digunakan untuk merekam status login dan identitas user ke SharedPreferences, sehingga aplikasi tahu kalau user masih login meskipun aplikasi ditutup lalu dibuka lagi.
    
    <img width="371" height="50" alt="image" src="https://github.com/user-attachments/assets/f8da449f-06e9-4a93-b8bb-7a75f4d28c0e" />

 - pubspec.yaml
   shared_preferences: ^2.2.2 ditambahkan supaya aplikasi bisa menyimpan status login di memori lokal (storage). Saat aplikasi dibuka lagi, sistem akan cek data itu. Kalau masih ada → user langsung masuk ke HomePage tanpa login ulang.
   
   <img width="214" height="62" alt="image" src="https://github.com/user-attachments/assets/59901c1d-e82e-47a8-9352-8d33d1529b5d" />

 menyimpan sesi login saat di refresh atau ditutup tidak perlu login lagi hasilnya seperti dibawah:

<img width="1908" height="1016" alt="Screenshot 2025-09-15 154352" src="https://github.com/user-attachments/assets/875e6971-edc1-44d5-98bc-2c44a1d5395f" />


 
   



   
     

     

   
   





       



  


  

  
  


    






