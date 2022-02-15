# Homework 8.3

Плейбук устанавливает на виртуальные машины сервиса yandex.cloud инструменты: ELK, Kibana, Filebeat
* В разделе group_vars описаны версии всех инструментов чтобы они были идентичны.
* В tamplates указаны шаблоны с описанием как будут связываться друг с другом инструменты, где будут распологаться файлы 
логов для ELK
* В hosts перечислены хосты и указаны публичные адреса вируальных машин

site.yml выполняет плей всех инструментов, где происходит скачивание и установка и примение условий шаблонов

Ссылка на [playbook](https://github.com/Evgeniy-Nikolskiy/mnt-11/tree/main/hw83/playbook)

Результат:
![screen1](https://raw.githubusercontent.com/Evgeniy-Nikolskiy/mnt-11/main/hw83/assets/831.png)