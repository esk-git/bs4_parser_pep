# Проект парсинга
Парсер, поможет быть в курсе важных изменений между основными версиями [Python](https://docs.python.org/3/):
- соберёт ссылки на статьи о нововведениях и достанет из них справочную информацию
- актуальную документацию
- статус и количество всех стандартов [PEP](https://peps.python.org/)
## Как запустить проект
- Клонировать репозиторий
```
https://github.com/esk-git/bs4_parser_pep.git
```
```
cd bs4_parser_pep
```

- Cоздать и активировать виртуальное окружение:

```
python3 -m venv venv
```

```
source venv/bin/activate
```

- Установить зависимости из файла requirements.txt:

```
python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```
### Для запуска программы нужно указать один из следующих аргументов:
- whats-new (напечатает ссылку на актуальные версии Python, и укажет автора)
- latest-versions (напечатает ссылку на документацию актуальных версий Python и их статус)
- download (скачает документацию последней версии Python)
- pep (напечатает статус и количество всех стандартов PEP)
### Примеры команд:
Вывести справку
```
python src/main.py pep -h
```
Создаст csv файл в папке ./results с таблицей из двух колонок: «Статус» и «Количество»:
```
python main.py pep -o file
```
#### Автор
Каликов Евгений
