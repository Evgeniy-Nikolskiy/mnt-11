## Homework 8.2

[Playbook](https://github.com/Evgeniy-Nikolskiy/mnt-11/tree/main/hw82/playbook) скачивает и устанавливает следующие инструменты: Java, ELK, Kibana.  
Основные пункты:
* скачать архив инструмента в расположение /tmp
* создать отдельную директорию и разархивировать инструмент; --strip-components=1 не даст плодить файлы при повторном запуске плейбука
* тег проставляется в соответствии с названием инструмента
* Согласно шаблону описывается переменная окружения

Мной было принято решение отредактировать файл [inventory/prod.yml](https://github.com/Evgeniy-Nikolskiy/mnt-11/blob/main/hw82/playbook/inventory/prod.yml) в сторону локального подключения.
Это было сделано из соображений простоты реализации, с Docker контейнером была отработка в предыдущем ДЗ. Хотел больше времени уделить флагам для запуска и проверки плейбука. Надеюсь такой вариант выполнения тоже приемлем.

Конечный результат выполнения команды: ansible-playbook -i inventory/prod.yml site.yml --diff

![screen1](https://raw.githubusercontent.com/Evgeniy-Nikolskiy/mnt-11/main/hw82/assets/Screenshot%20from%202022-02-09%2021-55-44.png)

