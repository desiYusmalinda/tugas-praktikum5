kelas  : TK2B

Nim    :09030182428014


1. Eksekusi profil
   
   a). Edit file profile /etc/profile dan tampilkan pesan,
   
   <img width="332" alt="desi1A" src="https://github.com/user-attachments/assets/9247109a-4083-4e22-baa3-7e01db3d69a8" />

   b). Ganti nama /home/mahasiswa dengan nama anda sendiri. pada setiap file tersebut, cantumkan instruksi echo
   
   ![WhatsApp Image 2025-04-13 at 17 22 07_0c7d088d](https://github.com/user-attachments/assets/108e4c11-4389-4a0d-9e24-15954830f241)


   ![WhatsApp Image 2025-04-13 at 17 22 32_11b0d3c8](https://github.com/user-attachments/assets/b7f5dcdd-d280-42c4-816a-0e5160ece564)


   ![WhatsApp Image 2025-04-13 at 17 26 06_ae3f5e55](https://github.com/user-attachments/assets/12268643-4dd4-40b3-bee5-ba80c3dcd3c1)


   ![WhatsApp Image 2025-04-13 at 17 25 30_17d50aa7](https://github.com/user-attachments/assets/ae6dd158-74ed-4cd1-a77b-aac02c319e7b)


    c). -instruksi su linda
   
   <img width="271" alt="desi1C su linda" src="https://github.com/user-attachments/assets/e7fe509f-19d8-4516-84a8-9a4eb88d2769" />


       -instruksi su - linda


   <img width="467" alt="desi1C su - linda" src="https://github.com/user-attachments/assets/c767682e-bf5e-48ef-b7ef-b527f7f92e63" />


    Perbedaanya : terletak pada bagaimana lingkungan pengguna dikonfigurasi setelah perpindahan, jika menggunakan su linda maka hanya berpindah ke pengguna tersebut tanpa mengubah lingkungan secara penuh, direktori kerja tetap di tempat sebelumnya dan variabel lingkungan seperti $PATH serta $HOME masih mengikuti pengguna sebelumnya, sedangkan jika menggunakan su - linda maka perpindahan dilakukan secara penuh seperti simulasi login baru, direktori kerja akan berubah ke /home/linda dan variabel lingkungan akan diperbarui sesuai dengan pengguna linda.



2. Prompt String (PS)
   
  a). Edit file .bash_profile, ganti prompt PS1 dengan '>'
  
<img width="70" alt="desi2A" src="https://github.com/user-attachments/assets/f1245a1e-6769-4f59-9c84-43d3dc602810" />

  
  b). Eksperimen hasil PS1
  
  <img width="199" alt="desi2B" src="https://github.com/user-attachments/assets/dfd1bc81-84e3-4423-be78-5c82ad714e57" />



3. Log out
   
   <img width="266" alt="desi3A" src="https://github.com/user-attachments/assets/024d360f-0b1c-48af-9c23-f3cc8a8c4001" />



4. Bash Script

   hasil jalankan script tersebut : -$ ./p1.sh ; ./p3.sh ; ./p2.sh
   
   <img width="307" alt="desi4A" src="https://github.com/user-attachments/assets/ffa6ae8f-7500-421a-87db-3d1a10958127" />
   

   -$ ./p1.sh &
   
   <img width="272" alt="desi4B" src="https://github.com/user-attachments/assets/6a5a704a-4cf4-4d10-9e04-c3bcf9180840" />


   -$ ./p1.sh $ ./p2.sh & ./p3.sh &
   
   <img width="300" alt="desi4C" src="https://github.com/user-attachments/assets/caf31c49-d336-4a1b-8497-a80da7eefe17" />


  -$ ( ./p1.sh ; ./p3.sh ) &
  
  <img width="283" alt="desi4D" src="https://github.com/user-attachments/assets/ba919229-1b58-464e-bd8d-9b434b85aaab" />



5. Jobs
   
  Hasil program yang di jalankan
  
-$ jobs

<img width="377" alt="desi5 jobs" src="https://github.com/user-attachments/assets/d0eff0cf-2d82-40ec-b9f4-1a0189761d05" />


-$ find / -print > files 2>/dev/null &

<img width="340" alt="desi5 find" src="https://github.com/user-attachments/assets/be8996ca-0b6f-49e6-bce3-97ac42f111cd" />


-$ jobs

<img width="377" alt="desi5 jobs" src="https://github.com/user-attachments/assets/485c8692-baee-4101-b003-4849171a8a03" />


-$ fg %1

<img width="244" alt="desi5 fg %1" src="https://github.com/user-attachments/assets/9d732607-57ab-4b6b-977b-2e644214dd1e" />


-$ bg

<img width="197" alt="desi5 bg" src="https://github.com/user-attachments/assets/6e3aaceb-1c67-459c-8ca9-2121f5b93860" />


Stop program background dengan utilitas kill

-$ ps x

<img width="286" alt="desi5 px" src="https://github.com/user-attachments/assets/42161563-e2fe-40d9-9660-5996dc89c2ed" />


-$ kill [Nomor PID]

<img width="325" alt="desi5 kill" src="https://github.com/user-attachments/assets/3256beec-d362-422d-afc9-564d02ced6ce" />



6. History
   
   a). Ganti nilai HISTSIZE dari 1000 menjadi 20
   
    -$ HISTSIZE=20
   
   <img width="218" alt="desi6 histsize" src="https://github.com/user-attachments/assets/05bc97a4-6ecf-441a-a38c-38cef4cc6640" />


   -$ history
   
   <img width="181" alt="desi6 history" src="https://github.com/user-attachments/assets/d3d87eb4-28df-483b-b901-93baff01de1b" />


   b). Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan
   
     -$ !-5
   
   <img width="158" alt="desi6 !-5" src="https://github.com/user-attachments/assets/cb0fdd7a-2a4d-4d1d-b5d0-b2b3e45abb1f" />


    c). Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer
   
      -$ !!
   
      <img width="173" alt="desi6 !!" src="https://github.com/user-attachments/assets/46c25164-7041-4ad2-bbd8-62cf6624a9b9" />


   d). Ulangi instruksi dengan bufer nomor 150
   
     -$ !150
   
     ![desi6 !150](https://github.com/user-attachments/assets/83380245-0db6-46ad-b28c-26641df4500b)

   
  e). Ulangi instruksi dengan prefix "ls"
  
    -$ !ls
    
    <img width="319" alt="desi6 !ls" src="https://github.com/user-attachments/assets/0961aac5-3f1a-4577-961c-0f0856b78f02" />
