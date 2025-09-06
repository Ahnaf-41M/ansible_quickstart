# ansible-docker-demo

Installs Docker on a managed Ubuntu container.

## Inventory

`inventories/dev/hosts.yml` points to a local Ubuntu container on port 2222.

## Quickstart

```bash
# (optional) Use a virtual env
python3 -m venv .venv && source .venv/bin/activate
pip install --upgrade pip ansible

# Sanity check: can Ansible reach the host?
ansible all -m ping

# Run the playbook
ansible-playbook playbooks/install-docker.yml

# Verify Docker on the managed node
ssh -i ~/.ssh/ansible -p 2222 ansible@127.0.0.1 'docker --version && docker run --rm hello-world'
```
