<p align="center">
  <img src="https://raw.githubusercontent.com/Finsys/dockhand/main/src/images/logo.webp" alt="Dockhand" width="300">
</p>

<p align="center">
  <strong>Modern Docker Management UI</strong>
</p>

<p align="center">
  <a href="https://dockhand.pro">Website</a> •
  <a href="https://dockhand.pro/manual">Documentation</a> •
  <a href="#license">License</a>
</p>

---

**Use**
```bash
rm -fr /opt/stacks/dockhand
mkdir -p /opt/stacks/dockhand
git clone https://github.com/FinchTechSoCal/docker-dockhand.git /opt/stacks/dockhand
sed -i 's;YourOwnSecretKey;'$(openssl rand -base64 32)';g' /opt/stacks/dockhand/.env
sed -i 's;DOCKER_GID=998;'DOCKER_GID=$(stat -c '%g' /var/run/docker.sock)';g' /opt/stacks/dockhand/.env
```

**Run**
```bash
docker compose -f /opt/stacks/dockhand/docker-compose.yml up -d
```

---


**Find docker.sock GID**
```bash
stat -c '%g' /var/run/docker.sock
```


**Modify .env Further**
```bash
nano /opt/stacks/dockhand/.env
```




## Agent
[hawser](https://github.com/FinchTechSoCal/docker-hawser)

[hawser official](https://github.com/Finsys/hawser)

## Docs
[Github](https://github.com/Finsys/dockhand)