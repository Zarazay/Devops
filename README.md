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

Создание deployment и poda c контейнером (Контейнер базовый тестовый httpd):
> nano kuber-pod.yaml

> kubectl apply -f kuber-pod.yaml

(result2.jpg)
