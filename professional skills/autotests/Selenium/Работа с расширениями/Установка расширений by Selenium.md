можно выкачивать из стора с помощью расширения crx
после этого можно установить расширение в экземпляр браузера который запускаем для тестов. Для этого юзаем options:

options = webdriver.ChromeOptions()
options.add_extension("путь до расширения.crx")

https://github.com/konflic/python_qa_windows/blob/master/5_javascript/test_example.py

#автоматизация 
#selenium 

[[Extensions]]