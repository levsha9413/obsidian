Дока 
раздел Quick started.
Качаем [Configuration Manager](http://aerokube.com/cm/latest/) из [releases](https://github.com/aerokube/cm/releases/latest)

wget -O cm <link_to_cm_release> - скачать с переименованием 
chmod +x cm

Для работы необходим установленный докер.
запуск 
./cm selenoid start - в первый раз скачает все необходимые файлы и образы в ~/.aerokube/ (установилось в /root/.aerokube/selenoid/browsers.json)
и запустит селеноид в контейнере

можно юзать docker ps

./cm selenoid start/stop - старт/стоп контейнера Selenoid 
./cm selenoid status - статус контейнера Selenoid/Selenoid UI 
./cm selenoid-ui start/stop - старт/стоп контейнера Selenoid UI 
./cm selenoid-ui status - статус контейнера Selenoid UI