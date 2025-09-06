# ansible-quickstart

This repository demonstrates how to use **Ansible** to install Docker on a managed Ubuntu container.  
The controller node is your local machine, and the managed node is a Docker container running Ubuntu with SSH access.

---

## 📦 Prerequisites

- Docker installed on your local machine
- Python 3 & Ansible installed locally
  ```bash
  python3 -m venv .venv && source .venv/bin/activate
  pip install --upgrade pip ansible
  ```
