Убираем атрибут через js и проверяем (выключили disabled)
js_code = "$('#disabled')[0].disabled = false;"
browser.execute_script(js_code)
- можно всячески модифицировать страницу на ходу
https://github.com/konflic/python_qa_webelements/blob/master/4_javascript/test_undisable_button.py


можно взаимодействовать с shadow DOM
https://github.com/konflic/python_qa_webelements/blob/master/4_javascript/test_example_shadow.py




[[JS в Selenium]]
[[shadow DOM]]