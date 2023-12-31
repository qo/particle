# English

## Хотите читать на русском?

Тыкните [cюда](#русский)

# Русский

## Что это?

Это темплейт для создания приложений-виджетов на фреймворке [Electron](https://www.electronjs.org/)

## Кому это нужно?

Людям, которые незнакомы с Electron, но хотят, чтобы их веб-решение запускалось как виджет

## Требования

Для использования потребуется установленные `git`, `node` и `npm`

## Установка и запуск проекта

### Клонирование репозитория

`git clone https://github.com/qo/particle.git`

### Установка зависимостей

`cd particle && npm install`

### Запуск проекта

`npm run hello-world-example`

### Что дальше?

После запуска вы увидите, что веб-страница `examples/hello-world/renderer/index.html` отрисовалась как виджет

## Как начать использовать темплейт?

### Изучите структуру примера `hello-world`

Вы увидите, что в папке `examples/hello-world` расположены:

- файл `config.js`
- папка `src`

В файле `config.js` описаны параметры создаваемого окна (виджета)

В папке `src` в свою очередь расположены папки `main`, `preload` и `renderer`

### Прочитайте туториал по модели процессов в Electron

Такое расположение папок отражает архитектуру Electron-приложений. Чтобы понять, зачем это надо и как с этим работать придется почитать про [модель процессов в Electron](https://www.electronjs.org/docs/latest/tutorial/process-model). В корне проекта используется такое же расположение папок.

## Структура проекта

### Файл `config.js`

Здесь можно задать настройки создаваемого для виджета окна

#### Поля:

- `pathToIndexHtml`: путь к `index.html` (обязательно)
- `pathToPreloadJs`: путь к `preload.js` (обязательно)
- `width`: ширина окна
- `height`: высота окна
- `transparent`: прозрачность окна
- `frame`: рамка окна
- `autoHideMenuBar`: меню-бар окна
- `resizable`: можно ли менять размер окна
- `alwaysOnTop`: закреплено ли окно поверх всех других окон
- `skipTaskbar`: нужно ли показывать окно в панели задач

Все поля можно найти в [описании класса BrowserWindow](https://www.electronjs.org/docs/latest/api/browser-window)

### Файл `default-config.js`

Здесь хранятся стандартные настройки создаваемого для виджета окна. Эти настройки имеют меньший приоритет, чем `config.js`

### Папка `src`

Здесь хранятся исходники

### Папка `src/main`

Здесь хранятся исходники для создания окна

### Папка `src/preload`

Lorem ipsum

### Папка `examples`

Lorem ipsum
