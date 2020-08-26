# docker-nexus

```

dock build -t waltonmax/nexus:latest .

docker pull waltonmax/nexus:latest

docker run -d -p 8081:8081 \
    --name=nexus \
    --net=host \
    -v /data/nexus/data:/data/nexus \
    waltonmax/nexus:latest

#docker-compose
docker-compose up -d
进入容器
docker exec -it nexus bash
```

