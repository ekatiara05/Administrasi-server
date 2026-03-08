# Remote Instance with SSH putty

1. pastikan sudah install putty
![alt text](image-10.png)

2. konversi file Public Key dari .pem menjadi .ppk di putty
    - buka puttyGen
    - load file .pem
    - save as .appk
    ![alt text](image-11.png)


3. set Up Putty untuk Remote SSH
- buka apps Putty
- Isi IP Public sesuai instance
- Isi Port untuk SSH sesuai Security Group di Instance
- Isi Nama session agar saat connect lagi tinggal load saja
- load file .ppk (Klik SSH-> Auth -> Credentials ->load file .ppk)
- Kembali ke Session klik Save 
- Klik open 
- Masukan username sesuai instance
![alt text](image-12.png)
![alt text](image-13.png)
![alt text](image-15.png)

4. Sudo apt-get Update (Update OS) lanjut "sudo apt-get upgrade
![alt text](image-17.png)

5. Pembuktian Remote SSH secara visual

6. sudo shutdown now
![alt text](image-18.png)