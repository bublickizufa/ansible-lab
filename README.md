# ansible-lab

Лабораторная работа №5 (DevOps): установка и настройка nginx и PHP на удалённом хосте с помощью Ansible.

| Файл | Назначение |
|------|------------|
| `ansible.cfg` | настройки Ansible (инвентарь, проверка ключей хостов) |
| `hosts.ini` | инвентарь — управляемый хост `devops-node` (192.168.100.11) |
| `install.yml` | playbook: установка nginx и интерпретатора PHP |
| `nginx.yml` | playbook: настройка сервиса nginx (запуск и автозагрузка), стартовая страница |
| `files/index.html` | стартовая страница сайта |

Запуск:

```bash
ansible web -m ping
ansible-playbook install.yml
ansible-playbook nginx.yml
```
