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
rm -fr ~/appdata/stacks/dockhand
git clone https://github.com/FinchTechSoCal/docker-dockhand.git ~/appdata/stacks/dockhand
sed -i 's;/path/to/appdata/;'$HOME'/appdata/;g' ~/appdata/stacks/dockhand/.env
```

**Find docker.sock GID**
```bash
stat -c '%g' /var/run/docker.sock
```


**Modify .env Further**
```bash
nano ~/appdata/stacks/dockhand/.env
```

**Run**
```bash
docker compose -f ~/appdata/stacks/dockhand/docker-compose.yml up -d
```

## Agent
[hawser](https://github.com/FinchTechSoCal/docker-hawser)

[hawser official](https://github.com/Finsys/hawser)

## Docs
[Github](https://github.com/Finsys/dockhand)