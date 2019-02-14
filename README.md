# Настройка сервера ТТМ c Ansible
## Требования

1. Создать инвентарный файл hosts (взять за пример local-hosts)

        {host} ansible_user={username}

2. Убедиться, что на хостах установлен 'python2'

## Использование, на локальной машине

    $ ansible-playbook -i hosts deploy.yml --ask-become-pass

## Тестирование

1. Запустить Vagrant

        $ vagrant up setupserver01

2. Запустить ansible

        $ ansible-playbook -i local-hosts deploy.yml

3. Зайти по SSH на локальный сервер

        $ vagrant ssh setupserver01
