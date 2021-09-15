алерты - окна браузера с сообщениями 
бывают сообщения
бывают с подтверждением 

есть отдельный класс для взаимодействия с алертами

browser.switch_to_alert - устарел

alert = browser.switch_to.alert - лучше юзать этот метод

методы:
.text()
.send_keys()
.accept()

обычно алерты заменяют pop-up'ами чтобы было красиво
c попапами уже работаем как с обычными элементами



https://github.com/konflic/python_qa_windows/blob/master/0_alerts/test_alerts.py

https://www.techbeamers.com/handle-alert-popup-selenium-python/

#selenium 
#работа_с_окнами
#автоматизация 