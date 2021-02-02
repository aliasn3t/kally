# callittea  
Приложение для отлова обновлений в репозиториях Kallithea при отключенном API  

#### Подготовка к использованию  
###### 1) Установка зависимостей  
`py -m pip install -r requirements.txt`  
###### 2) Конфигурирование  
Параметры хранятся внутри json-файла конфигурации   

#### Запуск  
Запуск: `py main.py`  
Доступные параметры запуска приложения:  
`--help` - показать список параметров запуска  
`--config` - запуск приложения с другим файлом конфигурации *(по умолчанию: ./conf.d/config.json)*  
`--without-jenkins` - не передавать задачи сборки в Jenkins *(по умолчанию: 0)*  
`--without-telegram` - не использовать оповещения в Telegram *(по умолчанию: 0)*   
Пример использования: `py main.py --config watchdog.json --without-telegram 1`  
