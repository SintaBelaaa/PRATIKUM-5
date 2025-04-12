NAMA : sinta bela


NIM : 09030182428011

KELAS : TK.2B

1.Eksekusi profil

a).edit file profile /etc/profile dan tampilkan pesan

![17444263811747180715919173374771](https://github.com/user-attachments/assets/37209ad1-7e84-4c3a-9c9d-9873e95e9c99)


b).Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo.

![17444264665349019487986873171458](https://github.com/user-attachments/assets/0f3dd1c3-41f2-41c1-8500-aab35480a755)


c).-Instruksi su bela dan exit

![17444265183345405602900745945072](https://github.com/user-attachments/assets/1414b5fa-7d11-4da4-be8a-b64b3b3db7b2)



-instruksi su - bela dan exit 

![17444265669782837200063324431588](https://github.com/user-attachments/assets/28f34f3b-accf-4d2d-a2c8-c8d3184e1808)

Perbedaanya : terletak pada bagaimana lingkungan pengguna dikonfigurasi setelah perpindahan, jika menggunakan su bela maka hanya berpindah ke pengguna tersebut tanpa mengubah lingkungan secara penuh, direktori kerja tetap di tempat sebelumnya dan variabel lingkungan seperti $PATH serta $HOME masih mengikuti pengguna sebelumnya, sedangkan jika menggunakan su - bela maka perpindahan dilakukan secara penuh seperti simulasi login baru, direktori kerja akan berubah ke /home/bela dan variabel lingkungan akan diperbarui sesuai dengan pengguna bela.

2.Prompt String (PS)

a).Edit file .bash_profile, ganti prompt PS1 dengan ‘>’.

![17444266171851488871814959631255](https://github.com/user-attachments/assets/9c794f20-1cf6-479e-a7f0-117d22644cdf)

b).Eksperimen hasil PS1

![17444266658048836369763555263364](https://github.com/user-attachments/assets/3e3284b8-3dbd-402f-b06f-cccc2de3068d)


3.Log out

![1744426710904759135425148022926](https://github.com/user-attachments/assets/20c6e10d-2872-4b6b-acab-d42a316087b1)


4.Bash script

hasil jalankan script tersebut : -$ ./p1.sh ; ./p3.sh ; ./p2.sh

![17444267628886352806487697998830](https://github.com/user-attachments/assets/8a3a5ff9-551b-4cd5-bf3d-165654feea4d)


-$ ./p1.sh &

![17444268145426152994206505713141](https://github.com/user-attachments/assets/28d68344-83dc-4f93-a7e0-8d01f13295ff)


-$ ./p1.sh $ ./p2.sh & ./p3.sh &

![17444269047825094868811047024286](https://github.com/user-attachments/assets/c586a1ff-e4c0-4a71-ad62-dc45f3496598)


-$ ( ./p1.sh ; ./p3.sh ) &

![17444269608235693824298108697129](https://github.com/user-attachments/assets/1f14d967-d218-4b65-badb-0325e55693bb)


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


![17444268586124409911638394454669](https://github.com/user-attachments/assets/a1254bc7-d03d-42fe-8ae8-8400f870327e)
