### Задание

- Поднять minikube
- Создать контейнер
- Создать тестовый deployment из ngix

### Порядок выполнения работы

Поднятие minikube:

- Включить VT-x/AMD-V
- Установить Docker и выдать ему права
> sudo chmod 666 /var/run/docker.sock
- Установить Kubectl
- Создать кластер
> minikube start

(result1.jpg)

Создание контейнера:


