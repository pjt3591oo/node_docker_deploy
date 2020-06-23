# 노드 프로젝트 도커배포

* 빌드 - 이미지 생성

```sh
$ docker build -f Dockerfile -t node_pactice .
```

-t 옵션으로 전달된 이름으로 이미지 생성

* 컨테이너 생성

```sh
docker run -i -t --name node_helloworld -p 3000:3000 node_pactice
```

--name 옵션으로 전달된 이름으로 컨테이너 생성

* 컨테이너 생성

```sh
docker run -i -t --name node_helloworld -p 3000:3000 -d node_pactice
```

* 이외 기타기능

```sh
$ docker ps 

$ docker ps -a

$ docker images

$ docker stop [CONTAINER NAME OR ID]

$ docker rm [CONTAINER NAME OR ID]

$ docker logs [CONTAINER NAME OR ID]

$ docker exec

$ docker exec -it [CONTAINER NAME] /bin/bash

$ docker commit [CONTAINER NAME] [CREATED IMAGE NAME:TAG]
```