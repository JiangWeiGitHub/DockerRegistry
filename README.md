# DockerRegistry
docker run -d -p 5000:5000 --restart=always --name registry -v /your/path/name:/var/lib/registry registry:2<p>

docker pull ubuntu && docker tag ubuntu localhost:5000/ubuntu<p>
docker push localhost:5000/ubuntu<p>

docker pull owncloud && docker tag owncloud localhost:5000/owncloud<p>
docker push localhost:5000/owncloud<p>

docker run -d -p 80:80 owncloud<p>
browser: http://localhost/<p>

