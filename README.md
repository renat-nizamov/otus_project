# otus_project
Обучающий проект otus. Создан для обучения навыкам и политикам SRE.

# Description
Приложение, разворачиваемое в проекте, является учебным и позволяет вносить в базу данных задачи и отмечать их выполнение.

# Requirements
Windows 10, VirtualBox v6.1.26 или выше, Vagrant 2.2.18 и выше.

# Instalation
Скопируйте проект https://github.com/renat-nizamov/otus_project.git с помощью GIT или архивом.

Запустите PowerShell, перейдите в директорию проекта и выполните команду:
```
vagrant up
```
В ходе установки будет предложено выбрать интерфейс через который осуществляется выход в интернет.
```
==> default: Available bridged network interfaces:
1) Intel(R) Wi-Fi 6 AX201 160MHz
2) Hyper-V Virtual Ethernet Adapter
==> default: When choosing an interface, it is usually the one that is
==> default: being used to connect to the internet.
==> default:
    default: Which interface should the network bridge to?
```
Сделайте выбор согласно вашей конфигурации сети.

После окончания подготовки виртуальной среды подключитесь к ней командой:
```
vagrant ssh
```
После входа в виртуальную среду выполните команду для запуска приложения:
```
python3 ./flask-sqlite3-todo-crud/app.py
```
!!Не выключайте консоль PowerShell в которой произведен запуск приложения до окончания работы с ним.!!

После запуска приложение доступно по url:
```
http://localhost:5000/
``` 
