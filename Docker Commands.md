# Docker related commands

#basic linux commands
```sh
  $hostname
  $hostname -i

  $mkdir day02
  $cd day02
  $git clone "https://github.com/vnkt2005/Docker.git
  $cat $"Docker Commands.md"

  $ls -lrt
```

#Building a simple Docker imaage for simple python application

#test.py
```sh
  print("This is my first python image")
```

#Dockerfile
```sh
  FROM python
  WORKDIR /app
  COPY . /app
  CMD ["python3","test.py"]
```

```sh
  $docker build -t myimage .
  $docker images
  $docker run myimage
```

```sh
  $docker run container -d -p 3000:3000 test
  $docker container ls
  $docker container stop 123ef260521db3
```

```sh
  $ docker tag myimage vnkt2020/myimage
  $ docker push vnkt2020/myimage
  $ docker login -u "myusername" -p "mypassword" docker.io
  $ docker push projetofinal2_web
```
