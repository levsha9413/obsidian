Т.к. iframe представляет собой отдельный сайт в другом сайте, то для взаимодействия с ним, на него нужно переключиться также как с окнами.

Первый способ:
Получаем iframe элементы на странице:

frames = chrome.find_elements_by_css_selector("iframe") - возвращает фреймы в виде обычных вебэлементов


Переключаемся в первый iframe в списке
chrome.switch_to.frame(frames[0])

Второй способ :
Можно переключаться по значению атрибута name элемента iframe, например если name="Selenium":
chrome.switch_to.frame("Selenium")

Третий способ:
можно переключаться по индексу:
chrome.switch_to.frame(2) - второй айфрейм

Возврат:
дальше все методы будут применяться только к выбранному фрейму, чтобы вернуться на родительскую страницу:

chrome.switch_to.default_content()

[[Переключение между окнами]]

#автоматизация 
#selenium 

https://github.com/konflic/python_qa_windows/blob/master/1_iframes/iframe.py