# Ansible + Docker Lab

Este proyecto simula múltiples servidores usando Docker y los configura automáticamente con Ansible.

## Tecnologías usadas
- Docker
- Docker Compose
- Ansible
- Ubuntu

## Qué hace
- Levanta 2 contenedores (node1 y node2)
- Configura SSH
- Instala Nginx automáticamente
- Despliega una página web

## Cómo ejecutar

```bash
docker compose up --build -d
ansible-playbook -i inventory.ini playbook.yml -K
