________________________________________________

поиск элементов на странице с помощью js:
web_el = browser.execute_script("return $('#disabled')[0]")

использование скрипта js из отдельного файла:
with open("upload.js") as f:
	browser.execute_script(f.read())
https://github.com/konflic/python_qa_windows/blob/master/5_javascript/test_example.py
______________________________________________________

Убираем атрибут через js и проверяем (выключили disabled)
js_code = "$('#disabled')[0].disabled = false;"
browser.execute_script(js_code)

- можно всячески модифицировать страницу на ходу
https://github.com/konflic/python_qa_webelements/blob/master/4_javascript/test_undisable_button.py

______________________________________________________
можно взаимодействовать с shadow DOM
https://github.com/konflic/python_qa_webelements/blob/master/4_javascript/test_example_shadow.py

----------------------------------------------
взаимодействие с куками в localStorage и sessionStorage

driver.execute_script("localStorage.setItem(\"k1\", \"value1\")")

driver.execute_script("return sessionStorage.getItem("k");")



[[JS в Selenium]]
[[shadow DOM]]
[[Работа с куками]]