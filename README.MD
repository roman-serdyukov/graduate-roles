# Репозиторий для сборки roles в рамках дипломного проекта Netology по специальности "DecOps-инженер"
## Файл  requirements.yml
Настроен для скачивания следующих ролей:
- [reverse-proxy-role](https://github.com/roman-serdyukov/reverse-proxy-role)
- [db-mysql-role](https://github.com/roman-serdyukov/db-mysql-role)
- [apps-server-role](https://github.com/roman-serdyukov/apps-server-role)
- [gitlab-ci-role](https://github.com/roman-serdyukov/gitlab-ci-role)
- [monitoring-role](https://github.com/roman-serdyukov/monitoring-role)

Запустить командой:
``` 
ansible-galaxy role install -r requirements.yml -p roles
```
При повторном запуске добавить '--force'

## Playbook site.yml
Настроен для запуска ролей:
- reverse-proxy-role
- db-mysql-role
- apps-server-role
- gitlab-ci-role
- monitoring-role

## Перед запуском
- Необходимо развернуть инфраструктуру.

## Совместимость
Роли тестировались в ОС ubuntu 20.04