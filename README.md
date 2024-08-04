Лабораторная работа №13 по курсу NoSQL.

Задание:

Установить Tarantool Cartridge CLI
Создать шаблон приложения командой:
	cartridge create --name myapp
Собрать и запустить приложение:
	cartridge build
	cartridge start
Задать любую топологию кластера в UI и сделать bootstrap


Решение:

Развернута виртуальная машина. На ВМ установлен Tarantool и сопутствующие инструменты:
	curl -L https://tarantool.io/release/3/installer.sh | bash
	curl -L https://tarantool.io/release/2/installer.sh | sudo -E bash -s -- --repo-only
	apt install tt
	apt -y install tarantool
	apt install cartridge-cli
	apt install tarantool-common
Проверил версию картриджа
	cartridge version
Создал картридж
	cartridge build
Запустил картридж
	cartridge start
Перешел на web (http://hostIP:8081), создал топологию кластера и сделал bootstrap (см Кластер Tarantool.jpg)
