capabilitese = 
scrinResolution: - разрешение экрана
name: - именует тесты(сессию) чтобы можно было найти ее в ui когда на нем одновременно запускают тесты несколько человек/команд

selenoid:option{...}:

enableVnc: True - vnc-доступ к контейнеру с браузером enableVideo: True - запись видео 
enableLogs: True - сохранение логов сессии
sessionTimeout: 60s - пауза на брейкпоинт для дебага

~/.aerokube/selenoid - директорий, где лежит browsers.json, logs, videos

В доке есть скрипт для чистки видео, чтобы они не выжрали память, можно удалять прошедшие тесты.

/cm selenoid start --args "-limit=10" - увеличение количества сессий. расчет количества сессий чтобы было хорошо и не тормозило https://aerokube.com/selenoid/latest/#_resources_consumption (по умолчанию 5)