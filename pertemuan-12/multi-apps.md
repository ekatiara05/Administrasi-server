# Deploy Multi Apps CI/CD Docker

1. Start Instance di AWS
2. patching OS -> sudo apt update && sudo apt upgrade
3. Hapus layanan nginx dan uninstall -> sudo systemctl stop nginx && sudo systemctl disable nginx sudo apt remove nginx  nginx-common nginx-core 
4. check docker ps -la dan docker start compro_2388010047

5. Hpus layanan Mariadb dan unisntall -> sudo systemctl stop mariadb && sudo systemctl disable mariadb sudo apt remove mariadb-server mariadb-client mariadb-common
6. Testing Next.js + db menggunakan user bukan root pada local env

    - copy project digitech pada ptm6 kecuali folder .next, node_modules, sql kedalam folder
!   [alt text](image.png)

    - buat usercompro_2388010047 set jadi localhost pw= 12345
!   [alt text](image-1.png)

    - sesuaikan isi file .env di folder compro_2388010047 username sama pw databasenya

    - open terminal cd web-dinamis

    - npm i

    - npm run dev
!   [alt text](image-2.png)