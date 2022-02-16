Фактически это обертка над стандартной реализацией сокетов. Библиотека в python основана на библиотека в с, в библиотеке c более полная документация. 
вызов документации из консоли линукс -
man 2 socket
man getaddrinfo


Примеры работы с библиотекой https://github.com/konflic/python_qa_net2

import socket
help(socket) # функции и константы для работы с сетью 
>>> socket.gethostbyname('ya.ru') #получить ip по url
>>> socket.gethostbyname('localhost')


[[BSD Socket API]]