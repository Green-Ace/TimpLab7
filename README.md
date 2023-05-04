
sudo apt update

sudo apt -y install curl gnupg2 apt-transport-https software-properties-common ca-certificates  

curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -

echo "deb [arch=amd64] https://download.docker.com/linux/debian buster stable" | sudo tee  /etc/apt/sources.list.d/docker.list

sudo apt update

sudo apt install docker-ce docker-ce-cli containerd.io

systemctl start docker

docker version




![изображение](https://user-images.githubusercontent.com/112771063/236219546-a6458786-df8d-49eb-bb83-cef0d3763855.png)



sudo docker build -t hello_world . 



![изображение](https://user-images.githubusercontent.com/112771063/236223079-3f6d72c8-c5fc-4bfd-812d-20cfc11e5324.png)




docker run hello_world



![изображение](https://user-images.githubusercontent.com/112771063/236223226-048d5f8b-ca3c-4a04-a052-5ef532da0c67.png)


