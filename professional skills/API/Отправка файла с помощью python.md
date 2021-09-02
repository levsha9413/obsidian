with open (file.jpg, "rb") as f:
	requests.post(upload, data=f)
	
rb - чтение бинарного файла
upload - url адрес куда посылаем файл

используем [[requests]]
также можно грузить и чанками по аналогии [[Скачивание файла с помощью python]] но пример нет