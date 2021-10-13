
1.  Создаем сессию: curl -d '{"desiredCapabilities": {"browserName": "chrome"}}' -X POST http://localhost:4444/wd/hub/session

2.  Открываем url: curl -d '{"url": "https://ya.ru"}' -X POST http://localhost:4444/wd/hub/session/${SESSION}/url

3.  Получаем title: curl -X GET http://localhost:4444/wd/hub/session/${SESSION}/title
     
	Закрываем браузер: curl -X DELETE http://localhost:4444/wd/hub/session/${SESSION}/window**