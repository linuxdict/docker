This is Libreoffice headless based on Alpine 

Build it: 
git clone https://github.com/linuxdict/docker.git

cd docker/alpine/libreoffice

docker build -t alpine:libreoffice .

Run it:
docker run -d --name myoffice01 -p 8997:8997 alpine:libreoffice
