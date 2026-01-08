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
rm -fr ~/appdata/docker_files/dockhand
git clone https://github.com/FinchTechSoCal/docker-dockhand.git ~/appdata/docker_files/dockhand
```

**Find docker.sock GID**
```bash
stat -c '%g' /var/run/docker.sock
```


**Modify .env**
```bash
nano ~/appdata/docker_files/dockhand/.env
```

**Run**
```bash
docker compose -f ~/appdata/docker_files/dockhand/docker-compose.yml up -d
```

## Agent
[hawser](https://github.com/FinchTechSoCal/docker-hawser)
[hawser official](https://github.com/Finsys/hawser)

## Docs
[Github](https://github.com/Finsys/dockhand)