Пример https://github.com/konflic/python_qa_net2/blob/master/demo/socket_create.py

Сокет с явным указанием всех параметров

my_socket = socket.socket(family=socket.AF_INET, type=socket.SOCK_STREAM, proto=0)

Внутри:
Address family - тип сети
AF_INET для сетевого протокола IPv4 
AF_INET6 для IPv6 

_Socket type_ 
SOCK_STREAM (надёжная потокоориентированная служба TCP) 
SOCK_DGRAM (служба датаграмм или датаграммный сокет UDP)

Сокет можно распечатать чтобы посмотреть его параметры.