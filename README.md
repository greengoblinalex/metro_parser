# Metro parser

## Описание проекта
Данный проект представляет собой инструмент для извлечения данных о продуктах из интернет-магазина Metro и экспорта этих данных в формат Excel.

## Установка и настройка
1. Клонирование репозитория:

Сначала склонируйте репозиторий на свой компьютер:
```
git clone https://github.com/yourusername/yourproject.git
```

2. Установка зависимостей:

Перейдите в каталог проекта и установите необходимые зависимости, выполнив команду:
```
pip install -r requirements.txt
```

3. Настройка параметров:

Для настройки параметров запроса к API Metro используются следующие аргументы метода `fetch_products_data()` класса `MetroParser`:
* slug (int): Slug категории продуктов. По умолчанию - категория кофе.
* store_id (int): ID магазина Metro. По умолчанию - магазин в Москве.
* size (int): Количество продуктов, запрашиваемых за один запрос. По умолчанию - 100.
* from_ (int): Индекс начала списка продуктов. По умолчанию - 0.
* in_stock (bool): Флаг, указывающий на необходимость отображения только продуктов, находящихся в наличии. Если True, отображаются только продукты в наличии, если False - все продукты. По умолчанию - True.

## Использование
1. Запуск скрипта:

Запустите скрипт main.py:
```
python main.py
```

2. Получение данных:

Скрипт получит данные о продуктах из магазина Metro для указанных магазинов (Москва, Санкт-Петербург и т. д.), используя класс MetroParser, и сохранит их в файл Excel.

3. Экспорт в Excel:

Данные о продуктах будут экспортированы в файл Excel с указанным именем и путем.
