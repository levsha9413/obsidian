Стандартный модуль python для организации логов.
Дока: [https://docs.python.org/3/howto/logging.html](https://docs.python.org/3/howto/logging.html)

import logging

logging.basicConfig() - конфигуратор логов. Логер конфигурируется 1 раз, если строчек несколько сработает только самый первый.(паттерн синглтон?)

Если кинули сообщение и потом выполнили конфигурацию

logging.warning("Ahtung")
logging.basicConfig("param param") 

, то при первом выводе сообщения установится дефолтный конфиг и вторая строчка уже не сработает. 

Из за этой особености конфигурации logging не используется напрямую, в каждом модуле logging заворачивается в свою обертку логгер.
пример https://github.com/konflic/python_qa_logging/blob/master/0_logging/3_logging_compose.py


#логирование 
#python 
