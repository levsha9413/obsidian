чтобы в отчете видеть какое мы использовали окружение при тесте, нужно прописать это окружение в файл 
/allure-results/environment.properties

пример https://github.com/agridyaev/otus-allure/blob/master/allure-results/environment.properties

чтобы файлик формировался автоматически, нужно в conftest положить фикстуру get_environment

пример https://github.com/agridyaev/otus-allure/blob/master/conftest.py

или добавить парсинг из парматров в финалайзер (понятнее) 
https://github.com/agridyaev/otus-selenoid/blob/master/conftest.py
(путь до environment.properties указывать относительно файла теста, а не conftest)