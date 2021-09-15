from selenium.webdriver import ActionChains

actions = ActionChains(browser)

actions.click_and_hold(card_element).pause(0.5).move_to_element(zone_element).release() - создаем цепочку действий 

actions.perform() - запускаем цепочку 

полный пример https://github.com/konflic/python_qa_webelements/blob/master/3_action_chains/test_drag_and_drop.py

[[ActionChains]]