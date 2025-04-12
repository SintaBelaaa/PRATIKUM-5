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


![17444270030517885635191788625432](https://github.com/user-attachments/assets/93aed829-044a-412d-9f61-8613fd029a5c)

 -$ find / -print > files 2>/dev/null &

![17444270503066021272259541335805](https://github.com/user-attachments/assets/54ae749a-fb04-4fb0-bec2-38b8b919fdc8)


-$ jobs

![1744427181873921063580395138269](https://github.com/user-attachments/assets/bf2ab943-7383-46a5-a9b6-89a58f7bad78)


Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background

-$ fg %1

![1744427253338996042636908913141](https://github.com/user-attachments/assets/f64808c8-c27c-40b0-8a0f-b68836626552)


-$ bg

![17444273028238795719687939578870](https://github.com/user-attachments/assets/8e7fa08a-d94b-4689-8b47-77ed45ef24a9)


Stop program background dengan utilitas kil

-$ ps 

![1744427354546326733279709005076](https://github.com/user-attachments/assets/28a66fc8-2e8c-4c42-8eca-a10bbd889da7)


-$ kill [Nomor PID]


![17444274024337899592783639603559](https://github.com/user-attachments/assets/18811ff7-d663-4322-88cf-743bdb3dbb99)


6.History

a).Ganti nilai HISTSIZE dari 1000 menjadi 20

 -$ HISTSIZE=20


![17444274484963104256206214036269](https://github.com/user-attachments/assets/5729167b-3aef-405c-89db-6ff43fea51b2)



-$ history

![17444274850683177475633054194411](https://github.com/user-attachments/assets/81111623-10a2-4d81-b4fe-f29d29aa9c54)


b).Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan

   -$ !-5

![17444275439944419150981707155977](https://github.com/user-attachments/assets/8b9b5c2d-bc27-47e5-8e83-e4c53c7486fd)


c). Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer

   -$ !!

![17444275925176999861934823451127](https://github.com/user-attachments/assets/9fe13ca9-51db-4de0-a9b8-47353758c494)


e).Ulangi instruksi dengan prefix “ls”

   -$ !ls


![17444268586124409911638394454669](https://github.com/user-attachments/assets/a1254bc7-d03d-42fe-8ae8-8400f870327e)
