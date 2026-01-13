# Ansible Multi-Server Web Deployment

## 📌 Project Overview
This project demonstrates deploying a static website to multiple servers using Ansible.  
A single reusable playbook automates web server installation and website deployment.

## 🏗️ Architecture
- Control Node: WSL (Ansible)
- Managed Nodes: Ubuntu Docker containers
- Web Server: Nginx
- Access Method: SSH (key-based)
- Deployment Type: Multi-server using inventory

## ⚙️ What the Playbook Does
- Installs Nginx
- Deploys static website files
- Uses variables for reusability
- Uses handlers to reload Nginx only when content changes
- Ensures idempotent and repeatable deployments
- Deploys to multiple servers using a single playbook

## 🚀 How to Run
```bash
ansible-playbook -i inventory.ini deploy_v3.yml
