# Лабораторная работа 5
В этой ветке представлены материалы лабораторной работы 5. Установка и настройка всего обеспечена ansible-сценарием. На сервеах с haproxy обеспечивается балансировка в режиме round-robin. Проверена работа балансировки и отказоустойчивость.

## Для поднятия виртуальной машины:
>vagrant up

## Для запуска ansible-сценария:
>ansible-playbook nginx.yml

## Результат балансировки(представлены кастомные страницы веб-серверов):
<a href="https://ibb.co/jzfmnZR"><img src="https://i.ibb.co/NrC5cnS/webb1.jpg" alt="webb1" border="0"></a>

<a href="https://ibb.co/c2TCCM8"><img src="https://i.ibb.co/vLzQQgd/webb2.jpg" alt="webb2" border="0"></a>

## Проверка отказоустойчивости:
Проверка отказоучточивости заключалась в следующих действиях: c помощью команды ***ip a*** сделалось возможным узнать, на какую виртуальную машину назначен адрес 192.168.11.100(тем самым определив, какой сервер нужно выключить для проверки).Выключаем. Работа не изменилась,значит все отлично.

<a href="https://ibb.co/FX0vjgB"><img src="https://i.ibb.co/1MdVw89/otkaz.jpg" alt="otkaz" border="0"></a><br /><a target='_blank' href='https://imgbb.com/'></a><br />

<a href="https://ibb.co/jzfmnZR"><img src="https://i.ibb.co/NrC5cnS/webb1.jpg" alt="webb1" border="0"></a>

<a href="https://ibb.co/c2TCCM8"><img src="https://i.ibb.co/vLzQQgd/webb2.jpg" alt="webb2" border="0"></a>





