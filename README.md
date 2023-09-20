# Добро пожаловать в сокращение URL!
Данное приложение было написано в следующем стеке технологий:
1. Инструментарий, использующий спецификацию OpenAPI: [Swagger](https://swagger.io/).
2. Набор инструментов для контроля доступа к ресурсам и аутентификации: HTTP Basic Authentication.
3. Свободная реляционная система управления базами данных: [MySQL](https://www.mysql.com/).

# Инструкция по настройке.
Для того, чтобы использовать приложение, необходимо настроить локальный хостинг MySQL, к примеру, используя СУБД [phpMyAdmin](https://www.phpmyadmin.net/). В своём проекте я использовал сборку веб-сервера на основе Apache: [Wamp Server](https://www.wampserver.com/). После запуска сборки веб-сервера, по умолчанию MySQL находится на порту 3306.
Откройте файл $${\color{lightblue}"\stroki\src\main\resources\"}$$$${\color{blue}application.properties}$$$${\color{lightblue}"}$$, чтобы изменить некоторые строки для доступа к базе данных. Строки, которые можно изменить:
- $${\color{green}"spring.datasource.url="}$$ - это параметр для указания пути к базе данных. Протоколы $${\color{lightgreen}jdbc:mysql://}$$ оставьте по умолчанию. Поменяйте домен $${\color{lightgreen}localhost:3306/}$$, если адрес порта отличается от вашего - замените на свои цифры, если же база данных находится на сервере - то необходимо указать путь до неё. Наконец, замените путь к странице $${\color{lightgreen}stroki}$$, указав существующую базу данных на вашем хостинге/сервере. Затем импортируйте структуру таблиц из файла $${\color{lightblue}"\stroki\src\main\resources\"}$$$${\color{blue}stroki.sql}$$$${\color{lightblue}"}$$ в вашей СУБД.
- $${\color{green}"spring.datasource.username="}$$ - это параметр указания имени пользователя для доступа к базе данных. Укажите вашего пользователя после знака "=".
- $${\color{green}"spring.datasource.password="}$$ - это параметр указания пароля для доступа к базе данных для того пользователя, что был указан выше.
- Остальные параметры изменений не требуют.
После настройки приложения можно запускать проект в своей IDE, а затем перейти [по ссылке для доступа к Swagger](http://localhost:8080/swagger-ui.html).

# Инструкция по эксплуатации.
$${\color{red}Здесь будет описан функционал проекта. Не забудь его дописать}$$
