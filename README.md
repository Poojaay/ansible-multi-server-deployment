#  Ansible Multi-Server Web Deployment

##  Project Overview
...

## 🏗️Architecture
...

##  Project Structure
...

## ⚙️What the Playbook Does  
- Installs Nginx
- Deploys static website files
- Uses variables for reusability
- Uses handlers to reload Nginx only when content changes
- Ensures idempotent and repeatable deployments
- Deploys to multiple servers using a single playbook

##  How to Run    AND THIS TOO
```bash
ansible-playbook -i inventory.ini deploy_v3.yml

