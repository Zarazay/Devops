# Devops

В репозитории предоставлен файл с YAML разметкой и HTML-файл, выводимый на странице сайта:

### Порядок выполнения работы
- установка ансибла:
> sudo apt install ansible

Сначала нужно в сетевых настройках выставить два адаптера: 
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
