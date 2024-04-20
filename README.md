### Задание

- Поднять minikube
- Создать контейнер
- Создать тестовый deployment из ngix

### Порядок выполнения работы

Поднятие minikube (С уже установленным docker):
> curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_amd64.deb
> sudo dpkg -i minikube_latest_amd64.deb
> minikube start

Выставить в сетевых настройках два адаптера: 
- Виртуальный адаптер хоста,
- NAT

Сгенерировать и установить ключ
> ssh-keygen -t rsa
> cat .ssh/id_rsa > ./ssh/authorized_keys

Создать .yml и .html
> mkdir lb
> touch playbook.yml
> touch index.html

Настроить правила проброса портов
Запустить yaml скрипт
> sudo ansible-playbook playbook.yml
