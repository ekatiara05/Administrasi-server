# Intro Docker Engine in Instance EC2 AWS

1. Install based Docker Documentation https://docs.docker.com/engine/install/ubuntu/
    - uninstall old version docker sudo apt remove $(dpkg --get-selections docker.io docker-compose docker-compose-v2 docker-doc podman-docker containerd runc | cut -f1)
    - install docke
    i. sudo apt-get update && sudo apt-get upgrade
    ii. add sertificate Repo sudo apt install ca-certificates curl sudo install -m 0755 -d /etc/apt/keyrings sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc sudo chmod a+r /etc/apt/keyrings/docker.asc
    iii. add Docker repository to APT sudo tee /etc/apt/sources.list.d/docker.sources <<EOF Types: deb URIs: https://download.docker.com/linux/ubuntu Suites: 
    {UBUNTU_CODENAME:-$VERSION_CODENAME}") Components: stable Architectures: $(dpkg --print-architecture) Signed-By: /etc/apt/keyrings/docker.asc EOF
    iv. Update OS sudo apt update
    v. Install the docker engine sudo apt install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
    vi. cek Installation sudo systemctl status docker
    ![alt text](image.png)
    
2. Registrasi Docker Hub
    - URL Docker Hub (https://hub.docker.com/repositories/ekatiara?_gl=1*txgeml*_gcl_au*NjkxMjMxNDUuMTc3NzI2MTE4Nw..*_ga*MzEwMTUyMjI0LjE3NzcyNjExODc.*_ga_XJWPQMJYHQ*czE3NzcyNjExODYkbzEkZzEkdDE3NzcyNjc5NzYkajIyJGwwJGgw)
    - Continue with Github
        ![alt text](image-1.png)

3. Create Repository for Docker
    - Klik Menu -> Hub -> Repositories
    - Klik Button New Repositories
    - isi nama repository dengan compro-2388010040 dan deskripsi Web App Statis Compro
    - Visibility Public
    - Pilih Create
        ![alt text](image-2.png)

4. Create token access

    - Klik Profile -> Settings -> personal access tokens
    - klik generate new token
    - isi deskripsi
    - expire date
![alt text](image-4.png)

5. Create Projek di local
        - buat folder compro_2388010040
        - masukkan file index.html
        - buat Dockerfile dengan isi sebagai berikut FROM nginx:alpine COPY index.html /usr/share/nginx/html/index.html EXPOSE 80

6. Push projek ke githup
    ![alt text](image-3.png)