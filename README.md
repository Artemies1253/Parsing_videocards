# Parsing_videocard
## Стек используемых текнологий: Python 3.9, Pony, BeautifulSoup, fake_useragent, requests, selenium.

Парсинг 4 крупных интернет магазинов на наличие видеокарт, все новые видеокарты заносятся в базу данных, на почту приходит сообщение о появление новой карты в магазине с информацией и сылкой на её покупку.

#### Перед запуском необходимо

Устанавливаем необходимые пакеты pip install -r requirements

Заполнить модуль модуль setting.py для отправления почты

Рекомендуется выставить фильтры на сайте интернет магазина и эту ссылку поставить как основную в парсер необходимого вам магазина, стандартно парситься все без фильтров


##### Для работы парсера DNS необходимо дополнительно скачать драйвер гугл хрома вашей версии с этой ссылки https://chromedriver.storage.googleapis.com/index.html , поместить его в корневую директорию проекта и выставить ваш user-agent.

#### Для запуска необходимо запустить модуль с интересующим вас магазином, например python manage.py parsing_DNS

###### P.S. Парсер баниться через сутки, рекомендую его использовать только для заполнения бд, для постоянного мониторинга нужно подкрутить поддержку прокси серверов и уменьшить тайминги 
