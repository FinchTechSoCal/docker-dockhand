# docker-dockhand
Docker management application

Use:
```bash
rm -fr ~/appdata/docker_files/dockhand
git clone https://github.com/FinchTechSoCal/docker-dockhand.git ~/appdata/docker_files/dockhand
```

Modify .env, then

```bash
docker compose -f ~/appdata/docker_files/dockhand/docker-compose.yml up -d
```

## Agent
[hawser](https://github.com/Finsys/hawser)
```bash
docker run -d \
  --name hawser \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -v /path/to/certs:/certs:ro \
  -p 2376:2376 \
  -e TLS_CERT=/certs/server.crt \
  -e TLS_KEY=/certs/server.key \
  -e TOKEN=your-secret-token \
  ghcr.io/finsys/hawser:latest
```

## Docs
[Github](https://github.com/Finsys/dockhand)