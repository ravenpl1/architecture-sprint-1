# Задание 1

## Уровень 1. Проектирование
Выбор сделан в пользу Single SPA т.к. неизвестен бэклог продукта, бюджет и вектор его развития. Сейчас используется один стэк - React, но могут появиться требования или команды использующие другие фреймворки/библиотеки, платформы сборок.
Соответственно применим три стратегии проектирования: вертикальная нарезка, автономность команд и изоляция микрофронтендов.

## Уровень 2. Планирование изменений
### 1. Микрофронтенд root-config (запуск)
App Shell приложение single-spa, так же включает в себя Header, Footer т.к. Header и Footer сейчас не развиты, по мере усложнения можно будет выделить в отдельный микрофронтенды. Root-config это точка входа в микрофронтенды, запуск происходит именно с него.

### 2. Микрофронтенд shared-dependencies
Указываются импорты (single-spa, react, react-dom).

### 3. Микрофронтенд styleguide
Сюда переносятся переиспользуемые(common) стили и js компоненты. Например стили PopUp, Content, Page

### 4. Микрофронтенд api
Здесь будет реализовываться связь с api бэкенда.

### 5. Микрофронтенд auth
Обеспечивает идентификацию/аутентификацию(логин/пароль) пользователя и получение токена авторизации.

### 6. Микрофронтенд register
Обеспечивает возможность зарегестрироваться пользователю

### 7. Микрофронтенд profile
Профиль пользователя

### 8. Микрофронтенд card
Карточки и места



# Задание 2
https://drive.google.com/file/d/10Sh6DlgWANBlY0XC32UVrPsrSCtoIANL/view?usp=sharing
