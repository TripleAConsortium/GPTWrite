# GPTWrite
📚 create gpt powered books with desired theme

Этот сценарий Python создает содержание книги и главы автоматически с помощью OpenAI API.

## Установка

1. Установите зависимости с помощью `pip`:

```bash
pip install -r requirements.txt
```

2. Добавьте [OpenAI API KEY](https://platform.openai.com/api-keys) в файл `.env`
 ```
 OPENAI_API_KEY=sk-***********************************************
 ```

Запустите сценарий, используя команду python3 app.py с соответствующими аргументами.
Использование
Примеры использования:

```bash
python3 app.py --title "android development" --description "книга по разработке андроид приложений. предназначена для новичков. последовательно освещает основные концепции разработки, паттерны проектирования, приемы проектирования UI и UX приложений" --tags java android development tutorial --details подробно --theme "руководство по разработке приложений для ОС андроид" --pages 50 --output android
```

```bash
python3 app.py --title "android development" --description "книга по разработке андроид приложений. предназначена для новичков. последовательно освещает основные концепции разработки, паттерны проектирования, приемы проектирования UI и UX приложений" --tags java android development tutorial --details "очень подробно" --theme "руководство по разработке приложений для ОС андроид" --pages 200 --output android --language Russian
```

```bash
python3 app.py --title "quality assurance" --description "книга является справочником для опытного QA инженера. в нее включены основные понятия QA, основные метрики качества, подходы к тестированию" --tags qa quality assurance cookbook  --details подробно --theme "справочник для QA инженера" --pages 200 --output qaguide --language Russian
```
пример [сгенерированной книги ](https://github.com/iampopovich/GPTWrite/releases/download/v1.1.0/qaguide.md)  
другие примеры можно найти в секции [releases](https://github.com/iampopovich/GPTWrite/releases)
<img width="1536" alt="Screenshot 2024-02-28 at 7 55 35 PM" src="https://github.com/iampopovich/GPTWrite/assets/23129441/67d81033-97d3-4c70-b855-e11677ed86d1">
<img width="1536" alt="Screenshot 2024-02-28 at 7 55 43 PM" src="https://github.com/iampopovich/GPTWrite/assets/23129441/ceddf7fa-a2f7-41e1-84c4-8827cd499d83">


Аргументы командной строки  
- `--theme` STRING: Тема книги (обязательный)
- `--description` STRING: Описание книги (обязательный)
- `--title` STRING: Название книги (опциональный)
- `--tags` LIST: Теги книги (опциональный)
- `--pages` INT: Количество страниц книги (опциональный)
- `--details` STRING: Детали книги (опциональный)
- `--language` STRING: Язык книги (опциональный)
- `--output` STRING: Имя выходного файла (обязательный)


