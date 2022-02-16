paramiko

Используем для аутентификации пароль Внутри /etc/ssh/sshd_config -> PasswordAuthentication yes/no 
Используем для аутентификации ключи С
оздаём файл ~/.ssh/authorized_keys Прописываем в него наш публичный ключ

Примеры кода:
https://github.com/nixuser/python_qa_net1/tree/master/examples/ssh

[[SSH]]