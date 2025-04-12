NAMA : sinta bela


NIM : 09030182428011

KELAS : TK.2B

1.Eksekusi profil

a).edit file profile /etc/profile dan tampilkan pesan

![17444263811747180715919173374771](https://github.com/user-attachments/assets/37209ad1-7e84-4c3a-9c9d-9873e95e9c99)


b).Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo.

(https://github.com/user-attachments/assets/df0c7740-16ba-4a84-8275-ea97c297cc7a)

c).-Instruksi su bela dan exit

(https://github.com/user-attachments/assets/ed5feb0a-3ecf-45a2-9d64-c8690b982866)


-instruksi su - bela dan exit 

(https://github.com/user-attachments/assets/00d40437-f57d-4d28-9dc2-6e7c8a90992c)

Perbedaanya : terletak pada bagaimana lingkungan pengguna dikonfigurasi setelah perpindahan, jika menggunakan su bela maka hanya berpindah ke pengguna tersebut tanpa mengubah lingkungan secara penuh, direktori kerja tetap di tempat sebelumnya dan variabel lingkungan seperti $PATH serta $HOME masih mengikuti pengguna sebelumnya, sedangkan jika menggunakan su - bela maka perpindahan dilakukan secara penuh seperti simulasi login baru, direktori kerja akan berubah ke /home/bela dan variabel lingkungan akan diperbarui sesuai dengan pengguna bela.

2.Prompt String (PS)

a).Edit file .bash_profile, ganti prompt PS1 dengan ‘>’.

(https://github.com/user-attachments/assets/a566f7df-7384-405e-bdef-084e3ee0318a)

b).Eksperimen hasil PS1

(https://github.com/user-attachments/assets/06c9cbc0-e202-4217-89dc-63e32c1d364b)

3.Log out

(https://github.com/user-attachments/assets/3c678939-8904-448f-8702-5320651885cc)

4.Bash script

hasil jalankan script tersebut : -$ ./p1.sh ; ./p3.sh ; ./p2.sh

(https://github.com/user-attachments/assets/44fcfaec-57ba-4741-899b-fde8f5552bce)

-$ ./p1.sh &

(https://github.com/user-attachments/assets/423e4284-e16f-4fb8-bec2-adca19bdebdb)

-$ ./p1.sh $ ./p2.sh & ./p3.sh &

(https://github.com/user-attachments/assets/117b9f77-c4ea-4b1f-9257-cb2f83271fc8)

-$ ( ./p1.sh ; ./p3.sh ) &

(https://github.com/user-attachments/assets/82823fe2-0724-4086-a981-356ef216285c)

5.Jobs

Hasil program yang dijalankan

-$ jobs

(https://github.com/user-attachments/assets/f2e430f3-5112-4b15-a084-07e3ee137939)

 -$ find / -print > files 2>/dev/null &

(https://github.com/user-attachments/assets/f6f702f9-91b4-459b-a33d-47cf756b1655)

-$ jobs

(https://github.com/user-attachments/assets/fdaa24f8-d6e3-4aa3-a304-dd6bd994eb2e)

Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background

-$ fg %1

(https://github.com/user-attachments/assets/1ee53572-c337-4b41-963f-3d23acb19420)

-$ bg

(https://github.com/user-attachments/assets/8c311bee-1679-48c0-b7b6-fdf29b05a0f5)

Stop program background dengan utilitas kil

-$ ps 

(https://github.com/user-attachments/assets/b45ba1c8-32fc-44d2-b7f9-0b5ce304c441)

-$ kill [Nomor PID]


(https://github.com/user-attachments/assets/4c7299a9-24e5-4f0e-b9d1-c54da7ae9f59)

6.History

a).Ganti nilai HISTSIZE dari 1000 menjadi 20

 -$ HISTSIZE=20


(https://github.com/user-attachments/assets/f8ec34d6-5a30-4ac9-9621-834b00d9a5c1)


-$ history

(https://github.com/user-attachments/assets/bfdf9aa0-81a9-42bd-b6a5-4ad30351223e)

b).Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan

   -$ !-5

(https://github.com/user-attachments/assets/06bb55fc-e142-4782-acde-056b83119dca)

c). Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer

   -$ !!

(https://github.com/user-attachments/assets/96b0f289-dd8f-4785-a450-5c05f528ab79)

e).Ulangi instruksi dengan prefix “ls”

   -$ !ls

(https://github.com/user-attachments/assets/451392ad-d641-4276-a082-7fee1d0a9d50)
