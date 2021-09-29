

**Commands to Dockerise python app**

1. docker build -t python-imdb .

2. docker run -it python-imdb


**Pushing to Dockerhub:**

1. docker run -dt --name "python-imdbcont" python-imdb:latest
docker container ls
copy container id

2. docker commit (CONTAINER ID) DOCKERUSERNAME/python-imdb:v1.1

3. docker login (login with dockerhub credentials)

4. docker push DOCKERUSERNAME/python-imdb:v1.1


Your docker image is now pushed to DockerHub :)


Extra: You can now use this image to run on your Kubernetes or another machine by doing docker pull or specifiying image when running pods.
