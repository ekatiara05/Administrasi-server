1. Pilih Menu All Services -> EC2
![alt text](image.png)

2. Di dalam Menu EC2 kita pilih instance
![alt text](image-1.png)

3. di dalam menu instance pilih launch instance
![alt text](image-2.png)

4. beri nama instance kita dengan format NIM_Server
![alt text](image-3.png)

5. kita pilih OS Sever untuk instance
![alt text](image-4.png)

6. pilih Resource instance T3.Micro (2VCPU, 1GB Memory)
![alt text](image-5.png)

7. Membuat key Pair, pilih New Pair, isi nama key, pilih RSA, format file .
![alt text](image-6.png)

8. Setting Kebijakan Keamanan / Security Group
    - Allow SSH -> Artinya membolehkan REmove SSH dari luar 
    - Allow HTTPS -> Artinya Instance bisa diakses dari protocol HTTPS
    - Allow HTTP -> Artinya Instance bisa diakses dari protocol HTTP
![alt text](image-7.png)

9. Selesai Set-up Pilih launch Instance
![alt text](image-8.png)

10. Pastikan Launch Instance Sukses
![alt text](image-9.png)

