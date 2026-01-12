# 🐳 WordPress Ansible Docker Provisioner

![Ansible](https://img.shields.io/badge/Ansible-EE0000?logo=ansible&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![WordPress](https://img.shields.io/badge/WordPress-2175A6?logo=wordpress&logoColor=white)
![Apache](https://img.shields.io/badge/Apache-D22128?logo=apache&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?logo=php&logoColor=white)

Automated provisioning of a **WordPress + MariaDB** stack on Ubuntu VMs using **Ansible** and **Docker**.  
Perfect for learning DevOps fundamentals or setting up a quick dev environment.

---

## ✨ Features

- ✅ Installs base tools (`mc`, `curl`, etc.) on target VMs  
- ✅ Fully automates **Docker Engine** and **Docker Compose Plugin** installation  
- ✅ Builds a custom **Apache + PHP** Docker image from scratch  
- ✅ Extends it to create a **WordPress-ready image**  
- ✅ Deploys a complete **WordPress + MariaDB** stack via `docker-compose`  
- ✅ Idempotent and reusable — run it as many times as you want!

---

## 🧰 Tech Stack

- **Configuration Management**: Ansible
- **Container Runtime**: Docker Engine
- **Orchestration**: Docker Compose Plugin (`docker compose`)
- **Web Stack**: Apache + PHP → WordPress
- **Database**: MariaDB (from Docker Hub)

---

## 🚀 Quick Start

1. **Clone the repo**
   ```bash
   git clone https://github.com/YOUR_USERNAME/wordpress-ansible-docker-provisioner.git
   cd wordpress-ansible-docker-provisioner
