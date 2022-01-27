### Docker Image load

```bash
docker load -i somethingImage.tar
```

### Docker 실행 중인 Container 조회

```bash
# 실행 중인 container만 조회 된다.
docker ps

# 중지된 container까지 조회
docker ps -a
```

### Docker Container 삭제

```bash
docker stop [container ID or container Name]
docker rm [container ID or container Name]
```

### Docker Container 시작 / 재시작 / 중지

```bash
docker start [container ID or container Name]

docker restart [container ID or container Name]

docker stop [container ID or container Name]
```

### Docker Container 접속 및 빠져나오기

```bash
# Container 접속
docker attach [container ID or container Name]
docker exec -it [containerID] [path]

# Container 빠져나오기
Ctrl + P + Q
```

### Docker File Copy

```bash
# host -> container
docker cp [hostPath] [containerId:{path}]

# container -> host 
docker cp [containerId:{path}] [hostPath]
```

### Docker container IP 조회

```bash
# 컨테이너 조회
docker inspect [containerID]

# 전체 조회
docker inspect bridge 
```