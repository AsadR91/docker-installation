```
Optionals
sudo usermod -aG docker $USER
newgrp docker

```

````
# Docker Installation Script for Ubuntu

This repository provides a simple and reliable shell script to install **Docker Engine**, **Docker Compose**, and related components on **Ubuntu-based systems** using Docker’s official repository.

## ✅ What This Script Does

- Updates system packages
- Installs required dependencies (`ca-certificates`, `curl`)
- Adds Docker’s official GPG key
- Adds the official Docker APT repository
- Installs:
  - Docker Engine (`docker-ce`)
  - Docker CLI (`docker-ce-cli`)
  - Containerd
  - Docker Buildx
  - Docker Compose plugin

## 📋 Supported Systems

- Ubuntu 20.04
- Ubuntu 22.04
- Ubuntu 24.04
- Other Ubuntu-based distributions with `apt`

## 🚀 How to Use

### 1. Clone the Repository
````

```bash
git clone git@github.com:AsadR91/docker-installation.git
cd docker-install-script
```



### 2. Make the Script Executable

```
chmod +x install-docker.sh
```

### 3. Run the Script

```
./install-docker.sh
```

> You may be prompted for your sudo password.

### 4. Verify Installation

```
docker --version
docker compose version
```

## 🔐 (Optional) Run Docker Without sudo

To allow your user to run Docker commands without `sudo`:

```
sudo usermod -aG docker $USER
newgrp docker
```

Log out and back in if required.

## 🧪 Test Docker

```
docker run hello-world
```

## 📦 Installed Packages

* `docker-ce`
* `docker-ce-cli`
* `containerd.io`
* `docker-buildx-plugin`
* `docker-compose-plugin`

## 🛡️ Security Notes

* Uses Docker’s official GPG key
* Uses signed APT repository
* No third-party scripts or curl | bash execution

## 📄 License

MIT License

````
