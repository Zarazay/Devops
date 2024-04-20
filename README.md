# Devops

В репозитории предоставлен файл с YAML разметкой и HTML-файл, выводимый на странице сайта:

### Порядок выполнения работы
- установка ансибла:
> sudo apt install ansible

Сначала нужно в сетевых настройках выставить два адаптера: 
- 1. Виртуальный адаптер хоста,
- 2. NAT
Сгенерировать и установить ключ
> ssh-keygen -t rsa
> cat .ssh/id_rsa > ./ssh/authorized_keys

- создать .yml и .html
> mkdir lb
> touch playbook.yml
> touch index.html
- настроить правила проброса портов
- запустить yaml скрипт
> sudo ansible-playbook playbook.yml
