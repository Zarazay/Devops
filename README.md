### Задание
Создать плейбук для сканирования запрошенных серверов при помощи nmap

### Порядок выполнения работы
> sudo apt install nmap

Создать invntory.ini с id и паролем (сменил виртуалку, ssh по паролю)
> touch inventory.ini
> cat >> inventory.ini

Создать плейбук
> touch pb_nmap.yml

Создать файл со сканируемыми серверами
> touch targets.txt

Выполнить плейбук
> ansible-playbook pb_nmap.yml -i inventory.ini --diff

Результат представлен в result.jpg
