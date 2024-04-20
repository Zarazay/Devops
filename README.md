### Задание

- Поднять minikube
- Создать контейнер
- Создать тестовый deployment из ngix

### Порядок выполнения работы

Поднятие minikube (С уже установленным docker):
> curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_amd64.deb

> sudo dpkg -i minikube_latest_amd64.deb
> minikube start



Настроить правила проброса портов
Запустить yaml скрипт
> sudo ansible-playbook playbook.yml
