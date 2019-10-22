# Установка и настройка Netbeans

## Установка
Скачать и установить NetBeans https://netbeans.org/

Можно скачать NetBeans с предустановленным jeddict https://jeddict.github.io/page.html?l=p/download

## Настройка

#### Настройки в файле конфигурации netbeans.conf

На Windows: В строку netbeans_default_options добавить -J-Dfile.encoding=UTF-8 (на linux UTF-8 берется из локали). Так же нужно в переменные среды добавить JAVA_TOOL_OPTIONS=-Dfile.encoding=UTF-8

Переключаем интерфейс на английский - так привычнее : в netbeans_default_options добавить --locale en_US 

## Установка и подключение Tomcat

Установка вручную: [скачать](https://tomcat.apache.org/download-90.cgi) и распаковать.

Подключение: 

Tools - Servers - Add server - Choose Server - Tomcat - Catalina Home - указать каталог с Tomcat. 

Для отладки удобно иметь свою конфигурацию сервера - крыжим Use Private Configuration Folder, 
указываем на пустой каталог (создать можно прямо из диалога выбора каталога). Заполняем имя и пароль пользователя, например ide и 123, этот пользователь будет использован для управления данным экземпляром Tomcat.

![](tomcat.png)

