[Demo](http://demo-ux.onedayessay.net/)

### Установка дополнительных инструментов для разработки wp-тем:
1. Автоматическая перезагрузка страниц в браузере во время работы с файлами WP-темы (css, php, images, etc.)
2. Компиляция less-файлов в css
3. Автоматическое добавление вендорных css-префиксов для кроссбраузерности
4. Сжатие изображений

### Предварительная установка программ
**Для реализации выше перечисленных задач, на компьютере должны быть предварительно установлены следующие программы:**

1. node.js (платформа JavaScript). Ссылка на инсталятор - https://nodejs.org/
2. gulp (инструмент сборки веб-приложений). Открыть консоль "node.js command prompt" и прописать команду:
npm install gulp -g
3. git (распределенная система управления версиями, удобная консоль для работы с gulp и управления npm-модулями). Ссылка на инсталятор для Windows https://git-scm.com/download/win

### Инструкция
**Инсталяция npm-модулей, которые выполняют все задачи, описанные в инструкции. Открыть git bush в папке с WP-темой и выполнить команду:**

npm install

*npm - это пакетный менеджер node.js, npm-модули - это js-скрипты для реализации различных задач.*

**В файл .gitignore, который находиться в корне сайта, добавить названия следующих файлов и папок:**

node_modules/
gulpfile.js
package.json
style.css.map

### Команды gulp
**Запуск автоматической перезагрузки страниц в браузере.**
**Компиляция less-файлов в css.**
**Добавление вендорных css-префиксов.**

gulp

*Перед выполнением команды необходимо в файле ".config.js" указать в переменной "domain" локальный домен (без http:// и конечного слеша /).**

***

**Сжатие изображений.**

gulp img