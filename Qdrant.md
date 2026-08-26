### Installation 
- create a storage folder
```
mkdir -p ~/qdrant_storage
```
- and then install

```
docker run -d \
  --name qdrant \
  --restart always \
  -p 6333:6333 \
  -p 6334:6334 \
  -v ~/qdrant_storage:/qdrant/storage \
  qdrant/qdrant:latest
```

- health check

```
curl http://localhost:6333/healthz
```

#### Docker commands for stopping and starting Qdrant

```
docker stop qdrant
```

```
docker start qdrant
```

- Restart Qdrant:

```
docker restart qdrant
```
- Check Status & Resource Usage:

```
docker ps -f name=qdrant
```
- View Live Logs:

```
docker logs -f qdrant
```
