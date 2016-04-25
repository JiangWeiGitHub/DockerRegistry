# DockerRegistry
docker run -d -p 5000:5000 --restart=always --name registry -v /your/path/name:/var/lib/registry registry:2

docker pull ubuntu && docker tag ubuntu localhost:5000/ubuntu
docker push localhost:5000/ubuntu

docker pull owncloud && docker tag owncloud localhost:5000/owncloud
docker push localhost:5000/owncloud

docker run -d -p 80:80 owncloud
browser: http://localhost/

