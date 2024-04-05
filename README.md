# Flask Blog

Этот проект представляет собой простое веб-приложение блога, созданное с использованием Flask, веб-фреймворка для Python. Он позволяет пользователям создавать, читать, обновлять и удалять записи в блоге.
Проект создан для Международного Университета Инновационных Технологий (IITU).

## Особенности

- Аутентификация пользователя: пользователи могут регистрироваться, входить и выходить из системы.
- Создание, чтение, обновление и удаление записей в блоге.
- Пользователи могут редактировать и удалять только свои собственные записи.
- Удобный интерфейс.

## Установка

1. Клонировать репозиторий:
git clone https://github.com/your_username/flask-blog.git

2. Перейти в директорию проекта:
cd flask-blog

3. Установить необходимые зависимости:
pip install -r requirements.txt

## Использование

1. Настроить приложение Flask:
export FLASK_APP=app.py
export FLASK_ENV=development

2. Инициализировать базу данных:
flask db init
flask db migrate
flask db upgrade

3. Запустить приложение Flask:
flask run

4. Откройте ваш веб-браузер и перейдите по адресу [http://localhost:5000](http://localhost:5000), чтобы просмотреть приложение.

## Как создавалось

1. Для начала необходимо создать новый проект в PyCharm, назовем его "__Blog on Flask__".
2. Затем внутри проекта создаем два файла: `app.py` и `templates.html`.
3. Для запуска нашей первой страницы в файле `app.py` мы пишем следующий код:

```python
from flask import Flask, render_template

app = Flask(__name__, template_folder='templates')

@app.route('/')
def index():
    return render_template('templates.html')

if __name__ == '__main__':
    app.run(debug=True)
````
значение debug=True после завершения создания сайта мы уберем на False, пока оно нам нужно для виденья какие ошибки могут возникать.
4. В templates.html мы пишем HTML код который будет служит основной нашего сайта, позже мы сможем добавлять в templates.html другие файлы типа html где сможем прописывать скрипт для кождой кнопки на сайте. Наш начальный код будет выглядеть примерно так:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flask Blog - README</title>
</head>
<body>
    <h1>Flask Blog</h1>

    <p>This project is a simple blog web application built using Flask, a Python web framework. It allows users to create, read, update, and delete blog posts.</p>

    <h2>Features</h2>
    <ul>
        <li>User authentication: Users can register, login, and logout.</li>
        <li>Create, read, update, and delete blog posts.</li>
        <li>Users can only edit and delete their own posts.</li>
        <li>User-friendly interface.</li>
    </ul>

    <h2>Installation</h2>
    <ol>
        <li>Clone the repository:</li>
    </ol>
    <pre><code>git clone https://github.com/your_username/flask-blog.git</code></pre>
    <ol start="2">
        <li>Navigate to the project directory:</li>
    </ol>
    <pre><code>cd flask-blog</code></pre>
    <ol start="3">
        <li>Install the required dependencies:</li>
    </ol>
    <pre><code>pip install -r requirements.txt</code></pre>

    <h2>Usage</h2>
    <ol>
        <li>Set up the Flask application:</li>
    </ol>
    <pre><code>export FLASK_APP=app.py
export FLASK_ENV=development</code></pre>
    <ol start="2">
        <li>Initialize the database:</li>
    </ol>
    <pre><code>flask db init
flask db migrate
flask db upgrade</code></pre>
    <ol start="3">
        <li>Run the Flask application:</li>
    </ol>
    <pre><code>flask run</code></pre>
    <ol start="4">
        <li>Open your web browser and go to <a href="http://localhost:5000">http://localhost:5000</a> to view the application.</li>
    </ol>

    <h2>Contributing</h2>
    <p>Contributions are welcome! Please feel free to fork the repository and submit pull requests to contribute to this project.</p>

    <h2>License</h2>
    <p>This project is licensed under the <a href="LICENSE">MIT License</a>.</p>

    <h2>Author</h2>
    <p>Zakariya</p>

    <h2>Acknowledgments</h2>
    <ul>
        <li>Special thanks to the Flask community for their excellent documentation and support.</li>
    </ul>
</body>
</html>
```
## Вклад в разработку

Приветствуются вклады! Пожалуйста, не стесняйтесь форкать репозиторий и отправлять запросы на объединение для внесения вклада в этот проект.
Также буду рад любой похвале или критике в своей проект, не стесняйтесь давать обратную связь!

## Лицензия

Этот проект распространяется под лицензией [MIT License](LICENSE).

## Автор

- Polevchishikov Zakariya (HELLPUSSY666)

## Благодарности

- Отдельная благодарность сообществу Flask за отличную документацию и поддержку.
- Так же очень благодарен своему практику и лектору в университете, за отличную подачу информации и совершенствование моих знаний в Python!

