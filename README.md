## Всем привет!

у нас есть три виртуальные машины 

1) web1
2) web2
3) rrobin

## Задача которую перед нами поставили:

Заставить сервера web1 и web2 работать по порту 8080, отдавать нам кастом страницу в гугле.
Сервер rrobin должен иметь балансировку нагрузки web1 и web2
И все это нужно запихнуть в ansible-сценарий, а потом создать плейбук
где расписать какую героическую роль будут иметь web1, web2 и rrobin.
И под конец этот самый плейбук должен создать страницу балансировки nginx rrobin для тех самых web1 и web2


## для начала вам понадобится образ вашей виртуальной машины centos7

1) вам нужно проверить вагрант статус командой - ``` vagrant status ```
2) Дальше вводим команду ``` vagrant up ```
3) И наконец запускаем сценарий командой - ``` ansible-playbook nginx ```


[vagrant up (поднимаем наши серваки)]

[ansible-playbook *название_вашего_сценария*.yml]


Готово!
проверить работу вы можете на странице http://192.168.11.113

<a href="https://ibb.co/kq8VjL5"><img src="https://ibb.co/kq8VjL5" alt="web1" border="0"></a>
