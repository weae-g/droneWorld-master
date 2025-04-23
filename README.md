## DroneWorld

Blog entries:

- [GameDev с three.js в современном вебе 🚀🎆](https://blog.openbloc.fr/gamedev-with-three-js-on-the-modern-web/)
- [Three.js и 3D-интерактивные анимации: обучающее руководство](https://blog.openbloc.fr/a-simple-and-flexible-render-loop-in-three-js/)

[Протестируйте игру в своем браузере](https://lab.openbloc.fr/droneWorld/)

[Следите за будущими обновлениями в Twitter с @maxmre](https://twitter.com/maxmre)

<img align="center" src="https://cdn.openbloc.fr/2018/04/Capture-du-2018-04-19-01-46-13.png" />

|                                                                     |                                                                     |
| :-----------------------------------------------------------------: | :-----------------------------------------------------------------: |
| <img src="https://pbs.twimg.com/media/Dh9azOpW0AIVLrl.jpg:large" /> | <img src="https://pbs.twimg.com/media/DfvLluyXkAIECoo.jpg:large" /> |
| <img src="https://pbs.twimg.com/media/Dh70d4WWsAAoGjC.jpg:large" /> | <img src="https://pbs.twimg.com/media/Dh70suSX0AAt9mG.jpg:large" /> |

## README по умолчанию для Create React App ниже

Этот проект был запущен с помощью [Create React App](https://github.com/facebookincubator/create-react-app).

Ниже вы найдете некоторую информацию о том, как выполнять общие задачи.<br>
Вы можете найти самую последнюю версию этого руководства [здесь](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md).

## Содержание

- [Обновление до новых версий](#updating-to-new-releases)
- [Отправка отзывов](#sending-feedback)
- [Структура папок](#folder-structure)
- [Доступные скрипты](#available-scripts)
  - [npm start](#npm-start)
  - [npm test](#npm-test)
  - [npm run build](#npm-run-build)
  - [npm run eject](#npm-run-eject)
- [Поддерживаемые браузеры](#supported-browsers)
- [Поддерживаемые языковые возможности и полифиллы](#supported-language-features-and-polyfills)
- [Подсветка синтаксиса в редакторе](#syntax-highlighting-in-the-editor)
- [Отображение вывода Lint в Редактор](#displaying-lint-output-in-the-editor)
- [Отладка в редакторе](#debugging-in-the-editor)
- [Автоматическое форматирование кода](#formatting-code-automatically)
- [Изменение страницы `<title>`](#changing-the-page-title)
- [Установка зависимости](#installing-a-dependency)
- [Импорт компонента](#importing-a-component)
- [Разделение кода](#code-splitting)
- [Добавление таблицы стилей](#adding-a-stylesheet)
- [Постобработка CSS](#post-processing-css)
- [Добавление препроцессора CSS (Sass, Less и т. д.)](#adding-a-css-preprocessor-sass-less-etc)
- [Добавление изображений, шрифтов и Файлы](#adding-images-fonts-and-files)
- [Использование папки `public`](#using-the-public-folder)
  - [Изменение HTML](#changing-the-html)
  - [Добавление ресурсов вне системы модулей](#adding-assets-outside-of-the-module-system)
  - [Когда использовать папку `public`](#when-to-use-the-public-folder)
- [Использование глобальных переменных](#using-global-variables)
- [Добавление Bootstrap](#adding-bootstrap)
  - [Использование пользовательской темы](#using-a-custom-theme)
- [Добавление потока](#adding-flow)
- [Добавление маршрутизатора](#adding-a-router)
- [Добавление пользовательских переменных среды](#adding-custom-environment-variables)
  - [Ссылки на переменные среды в HTML](#referencing-environment-variables-in-the-html)
  - [Добавление временных переменных среды в оболочке](#adding-temporary-environment-variables-in-your-shell)
  - [Добавление переменных среды разработки в `.env`](#adding-development-environment-variables-in-env)
- [Могу ли я использовать декораторы?](#can-i-use-decorators)
- [Извлечение данных с помощью запросов AJAX](#fetching-data-with-ajax-requests)
- [Интеграция с API Backend](#integrating-with-an-api-backend)
  - [Node](#node)
  - [Ruby on Rails](#ruby-on-rails)
- [Проксирование запросов API в разработке](#proxying-api-requests-in-development)
  - [Ошибки "Недопустимый заголовок хоста" после настройки прокси](#invalid-host-header-errors-after-configuring-proxy)
  - [Настройка прокси вручную](#configuring-the-proxy-manually)
  - [Настройка прокси-сервера WebSocket](#configuring-a-websocket-proxy)
- [Использование HTTPS в разработке](#using-https-in-development)
- [Создание динамических `<meta>` тегов на сервере](#generating-dynamic-meta-tags-on-the-server)
- [Предварительный рендеринг в статические HTML-файлы](#pre-rendering-into-static-html-files)
- [Внедрение данных с сервера на страницу](#injecting-data-from-the-server-into-the-page)
- [Выполнение тестов](#running-tests)
  - [Соглашения об именах файлов](#filename-conventions)
  - [Интерфейс командной строки](#command-line-interface)
  - [Интеграция контроля версий](#version-control-integration)
  - [Написание тестов](#writing-tests)
  - [Тестовые компоненты](#testing-components)
  - [Использование сторонних библиотек утверждений](#using-third-party-assertion-libraries)
  - [Инициализация тестовой среды](#initializing-test-environment)
  - [Фокусировка и исключение тестов](#focusing-and-exclusion-tests)
  - [Отчет о покрытии](#coverage-reporting)
  - [Непрерывная интеграция](#continuous-integration)
  - [Отключение jsdom](#disabling-jsdom)
  - [Снимок Тестирование](#snapshot-testing)
  - [Интеграция редактора](#editor-integration)
- [Отладочные тесты](#debugging-tests)
  - [Отладочные тесты в Chrome](#debugging-tests-in-chrome)
  - [Отладочные тесты в Visual Studio Code](#debugging-tests-in-visual-studio-code)
- [Разработка компонентов в изоляции](#developing-components-in-isolation)
  - [Начало работы с Storybook](#getting-started-with-storybook)
  - [Начало работы с Styleguidist](#getting-started-with-styleguidist)
- [Публикация компонентов в npm](#publishing-components-to-npm)
  - [Создание прогрессивного веб-приложения](#making-a-progressive-web-app)
  - [Отказ от кэширования](#opting-out-of-caching)
  - [Соображения, касающиеся офлайн-первым](#offline-first-considerations)
  - [Метаданные прогрессивного веб-приложения](#progressive-web-app-metadata)
- [Анализ размера пакета](#analyzing-the-bundle-size)
- [Развертывание](#deployment)
  - [Статический сервер](#static-server)
  - [Другие решения](#other-solutions)
  - [Обслуживание приложений с клиентской маршрутизацией](#serving-apps-with-client-side-routing)
  - [Создание относительных путей](#building-for-relative-paths)
  - [Azure](#azure)
  - [Firebase](#firebase)
  - [Страницы GitHub](#github-pages)
  - [Heroku](#heroku)
  - [Netlify](#netlify)
  - [Сейчас](#now)
  - [S3 и CloudFront](#s3-and-cloudfront)
  - [Surge](#surge)
- [Расширенная конфигурация](#advanced-configuration)
- [Устранение неполадок](#troubleshooting)
  - [`npm start` не обнаруживает изменения](#npm-start-doesnt-detect-changes)
  - [`npm test` зависает на macOS Sierra](#npm-test-hangs-on-macos-sierra)
  - [`npm run build` завершается слишком рано](#npm-run-build-exits-too-early)
  - [`npm run build` не удается на Heroku](#npm-run-build-fails-on-heroku)
  - [`npm run build` не удается минифицировать](#npm-run-build-fails-to-minify)
  - [Отсутствуют локали Moment.js](#momentjs-locales-are-missing)
- [Альтернативы Выбрасывание](#alternatives-to-ejecting)
- [Чего-то не хватает?](#something-missing)

## Обновление до новых релизов

Create React App делится на два пакета:

- `create-react-app` — это глобальная утилита командной строки, которую вы используете для создания новых проектов.
- `react-scripts` — это зависимость разработки в созданных проектах (включая этот).

Вам почти никогда не нужно обновлять сам `create-react-app`: он делегирует всю настройку `react-scripts`.

Когда вы запускаете `create-react-app`, он всегда создает проект с последней версией `react-scripts`, поэтому вы автоматически получите все новые функции и улучшения в новых созданных приложениях.

Чтобы обновить существующий проект до новой версии `react-scripts`, [откройте журнал изменений](https://github.com/facebookincubator/create-react-app/blob/master/CHANGELOG.md), найдите версию, на которой вы сейчас находитесь (если вы не уверены, проверьте `package.json` в этой папке), и примените инструкции по миграции для новых версий.

В большинстве случаев достаточно повысить версию `react-scripts` в `package.json` и запустить `npm install` в этой папке, но полезно ознакомиться с [журналом изменений](https://github.com/facebookincubator/create-react-app/blob/master/CHANGELOG.md) на предмет возможных критических изменений.

Мы обязуемся свести критические изменения к минимуму, чтобы вы могли безболезненно обновить `react-scripts`.

## Отправка отзыва

Мы всегда открыты для [ваших отзывов](https://github.com/facebookincubator/create-react-app/issues).

## Структура папок

После создания ваш проект должен выглядеть так:

```
my-app/
  README.md
  node_modules/
  package.json
  public/
    index.html
    favicon.ico
  src/
    App.css
    App.js
    App.test.js
    index.css
    index.js
    logo.svg
```

Для сборки проекта **эти файлы должны существовать с точными именами**:

- `public/index.html` — шаблон страницы;
- `src/index.js` — точка входа JavaScript.

Вы можете удалить или переименовать другие файлы.

Вы можете создать подкаталоги внутри `src`. Для более быстрой перестройки Webpack обрабатывает только файлы внутри `src`.<br>
Вам необходимо **поместить все файлы JS и CSS внутрь `src`**, иначе Webpack их не увидит.

Из `public/index.html` можно использовать только файлы внутри `public`.<br>
Читайте инструкции ниже по использованию ресурсов из JavaScript и HTML.

Однако вы можете создать больше каталогов верхнего уровня.<br>
Они не будут включены в производственную сборку, поэтому вы можете использовать их для таких вещей, как документация.

## Доступные скрипты

В каталоге проекта вы можете запустить:

### `npm start`

Запускает приложение в режиме разработки.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

Страница перезагрузится, если вы внесете изменения.<br>
Вы также увидите любые ошибки lint в консоли.

### `npm test`

Запускает тестовый раннер в режиме интерактивного просмотра.<br>
Дополнительную информацию см. в разделе о [запуске тестов](#running-tests).

### `npm run build`

Собирает приложение для производства в папку `build`.<br>
Он правильно объединяет React в режиме производства и оптимизирует сборку для лучшей производительности.

Сборка минимизирована, а имена файлов включают хэши.<br>
Ваше приложение готово к развертыванию!

Подробнее см. в разделе о [развертывании](#deployment).

### `npm run eject`

**Примечание: это односторонняя операция. После того, как вы `eject`, вы не сможете вернуться назад!**

Если вы не удовлетворены инструментом сборки и выбором конфигурации, вы можете `eject` в любое время. Эта команда удалит единственную зависимость сборки из вашего проекта.

Вместо этого она скопирует все файлы конфигурации и транзитивные зависимости (Webpack, Babel, ESLint и т. д.) прямо в ваш проект, чтобы вы имели полный контроль над ними. Все команды, кроме `eject`, по-прежнему будут работать, но они будут указывать на скопированные скрипты, чтобы вы могли их настраивать. На этом этапе вы сами по себе.

Вам никогда не нужно использовать `eject`. Курируемый набор функций подходит для небольших и средних развертываний, и вы не должны чувствовать себя обязанными использовать эту функцию. Однако мы понимаем, что этот инструмент будет бесполезен, если вы не сможете настроить его, когда будете к этому готовы.

## Поддерживаемые браузеры

По умолчанию сгенерированный проект использует последнюю версию React.

Вы можете обратиться [к документации React](https://reactjs.org/docs/react-dom.html#browser-support) для получения дополнительной информации о поддерживаемых браузерах.

## Поддерживаемые языковые возможности и полифиллы

Этот проект поддерживает надмножество новейшего стандарта JavaScript.<br>
В дополнение к синтаксическим возможностям [ES6](https://github.com/lukehoban/es6features) он также поддерживает:

- [Оператор возведения в степень](https://github.com/rwaldron/exponentiation-operator) (ES2016).
- [Async/await](https://github.com/tc39/ecmascript-asyncawait) (ES2017).
- [Свойства Object Rest/Spread](https://github.com/sebmarkbage/ecmascript-rest-spread) (предложение этапа 3).
- [Динамический импорт()](https://github.com/tc39/proposal-dynamic-import) (предложение этапа 3)
- [Поля классов и статические свойства](https://github.com/tc39/proposal-class-public-fields) (часть предложения этапа 3).
- Синтаксис [JSX](https://facebook.github.io/react/docs/introducing-jsx.html) и [Flow](https://flowtype.org/).

Узнайте больше о [различных этапах разработки предложений](https://babeljs.io/docs/plugins/#presets-stage-x-experimental-presets-).

Хотя мы рекомендуем использовать экспериментальные предложения с некоторой осторожностью, Facebook активно использует эти функции в коде продукта, поэтому мы намерены предоставить [codemods](https://medium.com/@cpojer/effective-javascript-codemods-5a6686bb46fb), если какие-либо из этих предложений изменятся в будущем.

Обратите внимание, что ** проект включает в себя только несколько ES6 [полифилл](https://en.wikipedia.org/wiki/Polyfill)**:

- [`Object.assign()`](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Object/assign) через [`object-assign`](https://github.com/sindresorhus/object-assign).
- [`Promise`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) через [`обещание`](https://github.com/then/promise).
- [`fetch()`](https://developer.mozilla.org/en/docs/Web/API/Fetch_API) через [`whatwg-fetch`](https://github.com/github/fetch).

Если вы используете какие-либо другие функции ES6+, для которых требуется поддержка во время выполнения (например, "Array.from()" или "Symbol"), убедитесь, что вы включили соответствующие полифиллы вручную или что браузеры, на которые вы ориентируетесь, уже поддерживают их.

Также обратите внимание, что использование некоторых новых синтаксических функций, таких как "for...of" или "[...nonArrayValue]", приводит к тому, что Babel выдает код, который зависит от функций среды выполнения ES6 и может не работать без polyfill. Если вы сомневаетесь, используйте [Babel REPL](https://babeljs.io/repl/), чтобы посмотреть, к чему сводится любой конкретный синтаксис.

## Подсветка синтаксиса в редакторе

Чтобы настроить подсветку синтаксиса в вашем любимом текстовом редакторе, перейдите на [соответствующую страницу документации по Babel](https://babeljs.io/docs/editors) и следуйте инструкциям. Здесь описаны некоторые из наиболее популярных редакторов.

## Отображение выходных данных Lint в редакторе

> Примечание: эта функция доступна в версиях `react-scripts@0.2.0` и выше.<br>
> Она также работает только с npm 3 или выше.

Некоторые редакторы, включая Sublime Text, Atom и Visual Studio Code, предоставляют плагины для ESLint.

Они не требуются для linting. Вы должны увидеть результаты linter прямо в вашем терминале, а также в консоли браузера. Однако, если вы предпочитаете, чтобы результаты lint отображались прямо в вашем редакторе, вы можете выполнить несколько дополнительных действий.

Сначала вам потребуется установить плагин ESLint для вашего редактора. Затем добавьте файл с именем ".eslintrc" в корневой каталог проекта:

```js
{
  "расширяет": "react-app"
}
```

Теперь ваш редактор должен сообщить о предупреждениях, связанных с linting.

Обратите внимание, что даже если вы продолжите редактировать свой файл `.eslintrc`, эти изменения ** повлияют только на интеграцию редактора**. Они не повлияют на вывод lint в терминале и в браузере. Это связано с тем, что приложение Create React намеренно содержит минимальный набор правил, которые позволяют находить распространенные ошибки.

Если вы хотите применить стиль программирования для своего проекта, рассмотрите возможность использования [Красивее](https://github.com/jlongster/prettier) вместо правил стиля ESLint.

## Отладка в редакторе

**В настоящее время эта функция поддерживается только [Visual Studio Code](https://code.visualstudio.com) и [WebStorm](https://www.jetbrains.com/webstorm/).**

Visual Studio Code и WebStorm поддерживают отладку "из коробки" с помощью Create React App. Это позволяет вам, как разработчику, писать и отлаживать свой код React, не выходя из редактора, и, что наиболее важно, обеспечивает непрерывный рабочий процесс разработки, при котором переключение контекста сведено к минимуму, поскольку вам не нужно переключаться между инструментами.

### Visual Studio Code

У вас должна быть установлена последняя версия [VS Code](https://code.visualstudio.com) и VS Code [Расширение для отладчика Chrome](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome).

Затем добавьте приведенный ниже блок в свой файл "launch.json" и поместите его в папку ".vscode" в корневом каталоге вашего приложения.

```json
{
	"version": "0.2.0",
	"configurations": [
		{
			"name": "Chrome",
			"type": "chrome",
			"request": "launch",
			"url": "http://localhost:3000",
			"webRoot": "${workspaceRoot}/src",
			"sourceMapPathOverrides": {
				"webpack:///src/*": "${webRoot}/*"
			}
		}
	]
}
```

> Примечание: URL-адрес может отличаться, если вы внесли изменения с помощью [переменных среды ХОСТА или порта] (#расширенная настройка).

Запустите приложение, запустив "npm start", и начните отладку в VS Code, нажав `F5` или щелкнув зеленый значок отладки. Теперь вы можете писать код, устанавливать точки останова, вносить изменения в код и отлаживать только что измененный код — и все это из своего редактора.

Возникли проблемы с отладкой VS Code? Пожалуйста, ознакомьтесь с их [руководством по устранению неполадок](https://github.com/Microsoft/vscode-chrome-debug/blob/master/README.md#troubleshooting).

### WebStorm

Вам потребуется установить расширение для Chrome [WebStorm](https://www.jetbrains.com/webstorm/) и [JetBrains IDE Support](https://chrome.google.com/webstore/detail/jetbrains-ide-support/hmhgeddbohgjknpmjagkdomcpobmllji).

В меню WebStorm `Выполнить" выберите "Редактировать конфигурации...". Затем нажмите "+" и выберите "Отладка JavaScript". Вставьте "http://localhost:3000` в поле URL и сохраните конфигурацию.

> Примечание: URL может отличаться, если вы внесли изменения с помощью [переменных среды хоста или порта] (#расширенная настройка).

Запустите свое приложение, запустив "npm start", затем нажмите "^D" в macOS или "F9" в Windows и Linux или щелкните зеленый значок отладки, чтобы начать отладку в WebStorm.

Таким же образом вы можете отлаживать свое приложение в IntelliJ IDEA Ultimate, PhpStorm, PyCharm Pro и RubyMine.

## Автоматическое форматирование кода

Prettier - это программа для самостоятельного формирования кода с поддержкой JavaScript, CSS и JSON. С помощью Prettier вы можете автоматически форматировать код, который вы пишете, чтобы обеспечить единый стиль кода в вашем проекте. Смотрите [Более красивую страницу на GitHub] (https://github.com/prettier/prettier) для получения дополнительной информации и посмотрите на эту [страницу, чтобы увидеть ее в действии] (https://prettier.github.io/prettier/).

Чтобы форматировать наш код всякий раз, когда мы выполняем фиксацию в git, нам нужно установить следующие зависимости:

```sh
npm install --save husky lint-staged prettier
```

В качестве альтернативы вы можете использовать "пряжу`:

```sh
yarn add husky lint-staged prettier
```

- `* `husky` упрощает использование git-перехватчиков, как если бы они были скриптами npm.
- "lint-staged" позволяет нам запускать скрипты для промежуточных файлов в git. Смотрите это [сообщение в блоге о lint-staged, чтобы узнать больше об этом](https://medium.com/@okonetchnikov/make-linting-great-again-f3890e1ad6b8).
- "красивее" - это средство форматирования JavaScript, которое мы будем запускать перед фиксацией.

Теперь мы можем убедиться, что каждый файл отформатирован правильно, добавив несколько строк в "package.json" в корневой папке проекта.

Добавьте следующую строку в раздел `скрипты`:

```diff
  "scripts": {
+   "precommit": "lint-staged",
    "start": "react-scripts start",
    "build": "react-scripts build",
```

Затем мы добавляем поле "поэтапный ввод" в `package.json`, например:

```diff
  "dependencies": {
    // ...
  },
+ "lint-staged": {
+   "src/**/*.{js,jsx,json,css}": [
+     "prettier --single-quote --write",
+     "git add"
+   ]
+ },
  "scripts": {
```

Теперь, всякий раз, когда вы делаете фиксацию, Prettier автоматически форматирует измененные файлы. Вы также можете запустить `./node\*modules/.bin/prettier - одинарные кавычки -написать "src/\*\*/\_.{js,jsx,json,css}", чтобы отформатировать весь ваш проект в первый раз.

Затем вы, возможно, захотите интегрировать Prettier в свой любимый редактор. Прочитайте раздел [Интеграция с редактором](https://prettier.io/docs/en/editors.html) на странице Prettier на GitHub.

## Измените название страницы.

Вы можете найти исходный HTML-файл в папке "public" созданного проекта. Вы можете отредактировать тег “<title>” в нем, чтобы изменить название с "React App" на что-либо другое.

Обратите внимание, что обычно вы не часто редактируете файлы в папке "public". Например, [добавление таблицы стилей](#adding-a-stylesheet) выполняется без изменения HTML-кода.

Если вам нужно динамически обновлять заголовок страницы в зависимости от содержимого, вы можете использовать API браузера [`document.title`](https://developer.mozilla.org/en-US/docs/Web/API/Document/title). Для более сложных сценариев, когда вы хотите изменить заголовок в React components, вы можете использовать [React Helmet](https://github.com/nfl/react-helmet), стороннюю библиотеку.

Если вы используете пользовательский сервер для своего приложения в рабочей среде и хотите изменить заголовок до того, как оно будет отправлено в браузер, вы можете последовать совету, приведенному в [этом разделе] (#генерация динамических мета-тегов на сервере). В качестве альтернативы, вы можете предварительно создать каждую страницу в виде статического HTML-файла, который затем загружает пакет JavaScript, описанный [здесь] (#предварительный рендеринг в статические html-файлы).

## Установка зависимости

Созданный проект включает в себя React и ReactDOM в качестве зависимостей. Он также включает набор скриптов, используемых Create React App в качестве зависимостей разработки. Вы можете установить другие зависимости (например, React Router) с помощью `npm`:

```sh
npm install --save react-router
```

В качестве альтернативы вы можете использовать `yarn`:

```sh
yarn add react-router
```

Это работает для любой библиотеки, а не только для "react-router".

## Импорт компонента

Благодаря Babel в этом проекте поддерживаются модули ES6.<br>
Хотя вы все еще можете использовать "require()" и "module.exports", мы рекомендуем вам использовать вместо этого ["import" и "export"](http://exploringjs.com/es6/ch_modules.html).

Например:

### `Button.js`

```js
import React, { Component } from 'react'

class Button extends Component {
	render() {
		// ...
	}
}

export default Button // Don’t forget to use export default!
```

### `DangerButton.js`

```js
import React, { Component } from 'react'
import Button from './Button' // Import a component from another file

class DangerButton extends Component {
	render() {
		return <Button color='red' />
	}
}

export default DangerButton
```

Помните о [различии между default и named, exports](http://stackoverflow.com/questions/36795819/react-native-es-6-when-should-i-use-curly-braces-for-import/36796281#36796281). Это часто приводит к ошибкам.

Мы рекомендуем вам использовать импорт и экспорт по умолчанию, когда модуль экспортирует только что-то одно (например, компонент). Это то, что вы получаете, когда используете "экспортировать кнопку по умолчанию" и "импортировать кнопку из "./Button".

Именованный экспорт полезен для служебных модулей, которые экспортируют несколько функций. В модуле может быть не более одного экспорта по умолчанию и столько именованных экспортов, сколько вам нужно.

Подробнее о модулях ES6:

- [Когда использовать фигурные скобки?](http://stackoverflow.com/questions/36795819/react-native-es-6-when-should-i-use-curly-braces-for-import/36796281#36796281)
- [Изучение ES6: модулей](http://exploringjs.com/es6/ch_modules.html)
- [Понимание ES6: модулей](https://leanpub.com/understandinges6/read#leanpub-auto-encapsulating-code-with-modules)

## Разделение кода

Вместо загрузки всего приложения до того, как пользователи смогут его использовать, разделение кода позволяет разделить ваш код на небольшие фрагменты, которые затем можно загружать по запросу.

Настройка этого проекта поддерживает разделение кода с помощью [динамического `импорта()`](http://2ality.com/2017/01/import-operator.html#loading-code-on-demand). Его [предложение](https://github.com/tc39/proposal-dynamic-import) находится на этапе 3. Функциональная форма `import()` принимает имя модуля в качестве аргумента и возвращает значение [`Promise`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise), которое всегда преобразуется в объект пространства имен модуля.

Вот пример:

### `moduleA.js`

```js
const moduleA = 'Hello'

export { moduleA }
```

### `App.js`

```js
import React, { Component } from 'react'

class App extends Component {
	handleClick = () => {
		import('./moduleA')
			.then(({ moduleA }) => {
				// Use moduleA
			})
			.catch(err => {
				// Handle failure
			})
	}

	render() {
		return (
			<div>
				<button onClick={this.handleClick}>Load</button>
			</div>
		)
	}
}

export default App
```

Это сделает `moduleA.js` и все его уникальные зависимости отдельным блоком, который загружается только после того, как пользователь нажмет кнопку "Загрузить".

Вы также можете использовать его с синтаксисом `async` / `await`, если вам так больше нравится.

### С помощью React Router

Если вы используете React Router, ознакомьтесь с [этим руководством] (http://serverless-stack.com/chapters/code-splitting-in-create-react-app.html) о том, как использовать разделение кода с его помощью. Вы можете найти соответствующий репозиторий на GitHub [here](https://github.com/AnomalyInnovations/serverless-stack-demo-client/tree/code-splitting-in-create-react-app).

Также ознакомьтесь с разделом [Разделение кода](https://reactjs.org/docs/code-splitting.html) в документации React.

## Добавление таблицы стилей

В этом проекте используется [Webpack](https://webpack.js.org/) для обработки всех ресурсов. Webpack предлагает пользовательский способ “расширения” концепции "импорта" за пределы JavaScript. Чтобы показать, что файл JavaScript зависит от файла CSS, вам необходимо ** импортировать CSS из файла JavaScript**:

### `Button.css`

```css
.Button {
	padding: 20px;
}
```

### `Button.js`

```js
import React, { Component } from 'react'
import './Button.css' // Tell Webpack that Button.js uses these styles

class Button extends Component {
	render() {
		// You can use them as regular CSS styles
		return <div className='Button' />
	}
}
```

**Это не требуется для React**, но многие пользователи находят эту функцию удобной. Вы можете прочитать о преимуществах этого подхода [here](https://medium.com/seek-ui-engineering/block-element-modifying-your-javascript-components-d7f99fcab52b). Однако вы должны знать, что это делает ваш код менее переносимым для других инструментов и сред сборки, чем Webpack.

В процессе разработки такое выражение зависимостей позволяет перезагружать ваши стили "на лету" по мере их редактирования. В процессе производства все файлы CSS будут объединены в один уменьшенный файл ".css" в выходных данных сборки.

Если вы заинтересованы в использовании семантики, специфичной для Webpack, вы можете поместить весь свой CSS прямо в "src/index.css". Он все равно будет импортирован из `src/index.js", но вы всегда можете удалить этот импорт, если позже перейдете на другой инструмент сборки.

## Постобработка CSS

Эта настройка проекта минимизирует ваш CSS и автоматически добавляет к нему префиксы поставщиков с помощью [Autoprefixer](https://github.com/postcss/autoprefixer), так что вам не нужно беспокоиться об этом.

Например, это:

```css
.App {
	display: flex;
	flex-direction: row;
	align-items: center;
}
```

becomes this:

```css
.App {
	display: -webkit-box;
	display: -ms-flexbox;
	display: flex;
	-webkit-box-orient: horizontal;
	-webkit-box-direction: normal;
	-ms-flex-direction: row;
	flex-direction: row;
	-webkit-box-align: center;
	-ms-flex-align: center;
	align-items: center;
}
```

Если вам по какой-либо причине необходимо отключить автоподстройку, [следуйте этому разделу](https://github.com/postcss/autoprefixer#disabling).

## Добавление CSS-препроцессора (Sass, Less и т.д.)

Как правило, мы рекомендуем вам не использовать одни и те же классы CSS повторно в разных компонентах. Например, вместо использования CSS-класса ".Button" в компонентах "<AcceptButton>" и "<RejectButton>" мы рекомендуем создать компонент "<Button>" со своими собственными стилями ".Button", которые могут использоваться как "<AcceptButton>", так и "<RejectButton>". отображать (но [не наследовать](https://facebook.github.io/react/docs/composition-vs-inheritance.html)).

Следование этому правилу часто делает CSS-препроцессоры менее полезными, поскольку такие функции, как микширование и вложенность, заменяются компоновкой. Однако вы можете интегрировать CSS-препроцессор, если считаете его полезным. В этом пошаговом руководстве мы будем использовать Sass, но вы также можете использовать Less или другую альтернативу.

Сначала давайте установим интерфейс командной строки для Sass:

```sh
npm install --save node-sass-chokidar
```

Alternatively you may use `yarn`:

```sh
yarn add node-sass-chokidar
```

Then in `package.json`, add the following lines to `scripts`:

```diff
   "scripts": {
+    "build-css": "node-sass-chokidar src/ -o src/",
+    "watch-css": "npm run build-css && node-sass-chokidar src/ -o src/ --watch --recursive",
     "start": "react-scripts start",
     "build": "react-scripts build",
     "test": "react-scripts test --env=jsdom",
```

> Примечание: Чтобы использовать другой препроцессор, замените команды "build-css" и "watch-css" в соответствии с документацией вашего препроцессора.

Теперь вы можете переименовать "src/App.css" в "src/App.scss`и запустить`npm run watch-css`. Наблюдатель найдет каждый файл Sass в подкаталогах "src" и создаст соответствующий файл CSS рядом с ним, в нашем случае перезаписав "src/App.css`. Поскольку "src/App.js` по-прежнему импортирует "src/App.css", стили становятся частью вашего приложения. Теперь вы можете редактировать "src/App.scss", и "src/App.css" будет восстановлен.

Чтобы обмениваться переменными между файлами Sass, вы можете использовать Sass imports. Например, "src/App.scss" и другие файлы стилей компонентов могут содержать "@import "./shared.scss";" с определениями переменных.

Чтобы включить импорт файлов без использования относительных путей, вы можете добавить параметр "--include-path" к команде в `package.json`.

```
"build-css": "node-sass-chokidar --include-path ./src --include-path ./node_modules src/ -o src/",
"watch-css": "npm run build-css && node-sass-chokidar --include-path ./src --include-path ./node_modules src/ -o src/ --watch --recursive",
```

This will allow you to do imports like

```scss
@import 'styles/_colors.scss'; // assuming a styles directory under src/
@import 'nprogress/nprogress'; // importing a css file from the nprogress node module
```

На этом этапе вы, возможно, захотите удалить все файлы CSS из системы управления версиями и добавить "src/\*_/_.css" в свой файл ".gitignore". Как правило, рекомендуется сохранять продукты сборки вне системы управления версиями.

В качестве заключительного шага, возможно, вам будет удобно запустить "watch-css" автоматически с помощью "npm start" и запустить "build-css" как часть "npm run build". Вы можете использовать оператор `&&` для последовательного выполнения двух сценариев. Однако кроссплатформенного способа параллельного запуска двух скриптов не существует, поэтому мы установим пакет для этого:

```sh
npm install --save npm-run-all
```

В качестве альтернативы вы можете использовать `yarn`:

```sh
yarn add npm-run-all
```

Затем мы можем изменить скрипты "start" и "build", включив в них команды препроцессора CSS:

```diff
   "scripts": {
     "build-css": "node-sass-chokidar src/ -o src/",
     "watch-css": "npm run build-css && node-sass-chokidar src/ -o src/ --watch --recursive",
-    "start": "react-scripts start",
-    "build": "react-scripts build",
+    "start-js": "react-scripts start",
+    "start": "npm-run-all -p watch-css start-js",
+    "build-js": "react-scripts build",
+    "build": "npm-run-all build-css build-js",
     "test": "react-scripts test --env=jsdom",
     "eject": "react-scripts eject"
   }
```

Теперь при запуске "npm start`и`npm run build" также создаются файлы Sass.

**Почему "node-sass-chokidar"?**

Сообщалось, что в "node-sass" возникают следующие проблемы:

- сообщалось, что при использовании node-sass -watch в определенных условиях возникают проблемы с производительностью при использовании на виртуальной машине или с помощью docker.

- Компиляция бесконечных стилей [#1939](https://github.com/facebookincubator/create-react-app/issues/1939)

- сообщалось, что у node-sass возникают проблемы с обнаружением новых файлов в каталоге [#1891](https://github.com/sass/node-sass/issues/1891)

здесь используется node-sass-chokidar для устранения этих проблем.

## Добавление изображений, шрифтов и файлов

В Webpack использование статических ресурсов, таких как изображения и шрифты, работает аналогично CSS.

Вы можете ** `импортировать` файл прямо в модуль JavaScript**. Это позволяет Webpack включить этот файл в пакет. В отличие от импорта CSS, при импорте файла вы получаете строковое значение. Это значение является конечным путем, на который вы можете ссылаться в своем коде, например, в качестве атрибута `src` для изображения или `href` для ссылки на PDF-файл.

Чтобы сократить количество запросов к серверу, при импорте изображений размером менее 10 000 байт вместо пути возвращается [URI данных](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/Data_URIs). Это относится к файлам со следующими расширениями: bmp, gif, jpg, jpeg и png. Файлы SVG исключены из-за [#1153](https://github.com/facebookincubator/create-react-app/issues/1153).

Вот пример:

```js
import React from 'react'
import logo from './logo.png' // Tell Webpack this JS file uses this image

console.log(logo) // /logo.84287d09.png

function Header() {
	// Import result is the URL of your image
	return <img src={logo} alt='Logo' />
}

export default Header
```

Это гарантирует, что при сборке проекта Webpack правильно переместит изображения в папку сборки и предоставит нам правильные пути.

Это также работает в CSS:

```css
.Logo {
	background-image: url(./logo.png);
}
```

Webpack находит все относительные ссылки на модули в CSS (они начинаются с `./`) и заменяет их конечными путями из скомпилированного пакета. Если вы допустите опечатку или случайно удалите важный файл, вы увидите ошибку компиляции, как при импорте несуществующего модуля JavaScript. Окончательные имена файлов в скомпилированном пакете генерируются Webpack из хэшей содержимого. Если содержимое файла изменится в будущем, Webpack присвоит ему другое имя в рабочей среде, так что вам не нужно беспокоиться о долгосрочном кэшировании ресурсов.

Пожалуйста, имейте в виду, что это также пользовательская функция Webpack.

**Она не требуется для React**, но многим людям она нравится (и React Native использует аналогичный механизм для изображений).
Альтернативный способ обработки статических ресурсов описан в следующем разделе.

## Использование `общедоступной` папки

> Note: this feature is available with `react-scripts@0.5.0` and higher.

### Изменение HTML-кода

В папке "public" находится HTML-файл, который можно изменить, например, на [задать заголовок страницы] (#изменение заголовка страницы).
Тег "<script>" со скомпилированным кодом будет добавлен к нему автоматически в процессе сборки.

### Добавление ресурсов за пределами системы модулей

Вы также можете добавить другие ресурсы в папку "public".

Обратите внимание, что обычно мы рекомендуем вам "импортировать" ресурсы в файлы JavaScript.
Например, смотрите разделы [добавление таблицы стилей] (#добавление таблицы стилей) и [добавление изображений и шрифтов] (#добавление изображений, шрифтов и файлов).
Этот механизм предоставляет ряд преимуществ:

- Скрипты и таблицы стилей сокращаются и объединяются вместе, чтобы избежать дополнительных сетевых запросов.
- Отсутствие файлов приводит к ошибкам компиляции, а не к ошибкам 404 для ваших пользователей.
- Имена результирующих файлов содержат хэши содержимого, поэтому вам не нужно беспокоиться о том, что браузеры будут кэшировать свои старые версии.

Однако есть ** запасной выход**, который вы можете использовать для добавления ресурса вне системы модулей.

Если вы поместите файл в папку "public", он не будет обработан Webpack. Вместо этого он будет скопирован в папку сборки нетронутым. Чтобы ссылаться на ресурсы в папке "public", вам нужно использовать специальную переменную под названием `PUBLIC_URL`.

Внутри `index.html" вы можете использовать ее следующим образом:

```html
<link rel="shortcut icon" href="%PUBLIC_URL%/favicon.ico" />
```

Только файлы внутри папки `public` будут доступны с префиксом `%PUBLIC_URL%`. Если вам нужно использовать файл из `src` или `node_modules`, вам нужно будет скопировать его туда, чтобы явно указать свое намерение сделать этот файл частью сборки.

Когда вы запускаете "npm run build", приложение Create React заменит "%PUBLIC_URL%" правильным абсолютным путем, чтобы ваш проект работал, даже если вы используете маршрутизацию на стороне клиента или размещаете его по некорневому URL-адресу.

В коде JavaScript вы можете использовать `process.env.PUBLIC_URL` для аналогичных целей:

```js
render() {
  // Note: this is an escape hatch and should be used sparingly!
  // Normally we recommend using `import` for getting asset URLs
  // as described in “Adding Images and Fonts” above this section.
  return <img src={process.env.PUBLIC_URL + '/img/logo.png'} />;
}
```

Имейте в виду недостатки этого подхода:

- Ни один из файлов в папке "public" не подвергается последующей обработке или уменьшению.
- Отсутствующие файлы не будут вызваны во время компиляции и приведут к ошибке 404 для ваших пользователей.
- Имена файлов результатов не будут содержать хэшей содержимого, поэтому вам нужно будет добавлять аргументы запроса или переименовывать их при каждом изменении.

### Когда использовать "общедоступную` папку

Обычно мы рекомендуем импортировать [таблицы стилей] (#добавление таблицы стилей), [изображения и шрифты] (#добавление изображений, шрифтов и файлов) из JavaScript.
`Общедоступная` папка полезна в качестве обходного пути для ряда менее распространенных случаев:

- В выходных данных сборки вам нужен файл с определенным именем, например [`manifest.webmanifest`](https://developer.mozilla.org/en-US/docs/Web/Manifest).
- У вас есть тысячи изображений, и вам нужно динамически ссылаться на пути к ним.
- Вы хотите включить небольшой скрипт, например [`pace.js`](http://github.hubspot.com/pace/docs/welcome/), за пределы встроенного кода.
- Некоторые библиотеки могут быть несовместимы с Webpack, и у вас нет другого выбора, кроме как включить их в качестве тега "<script>".

Обратите внимание, что если вы добавляете "<скрипт>", который объявляет глобальные переменные, вам также необходимо прочитать следующий раздел, посвященный их использованию.

## Использование глобальных переменных

Когда вы добавляете в HTML-файл скрипт, определяющий глобальные переменные, и пытаетесь использовать одну из этих переменных в коде, программа компоновки будет жаловаться, потому что не сможет увидеть определение переменной.

Вы можете избежать этого, прочитав глобальную переменную явно из объекта window, например:

```js
const $ = window.$
```

Это делает очевидным, что вы используете глобальную переменную намеренно, а не из-за опечатки.

В качестве альтернативы вы можете заставить линтер игнорировать любую строку, добавив после нее "// eslint-disable-line".

## Добавляем Bootstrap

Вам не обязательно использовать [React Bootstrap](https://react-bootstrap.github.io) вместе с React, но это популярная библиотека для интеграции Bootstrap с приложениями React. Если вам это нужно, вы можете интегрировать ее с Create React App, выполнив следующие действия:

Установите React Bootstrap и Bootstrap для начальной загрузки из npm. React Bootstrap не включает Bootstrap CSS, поэтому его также необходимо установить:

```sh
npm install --save react-bootstrap bootstrap@3
```

В качестве альтернативы вы можете использовать `yarn`:

```sh
yarn add react-bootstrap bootstrap@3
```

Импорт начальной загрузки CSS и при необходимости Bootstrap тему CSS в начало вашего файла `src/index.js` :

```js
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap/dist/css/bootstrap-theme.css'
// Put any other imports below so that CSS from your
// components takes precedence over default styles.
```

Импортируйте необходимые компоненты React Bootstrap из файла `src/App.js` или ваших пользовательских файлов компонентов:

```js
import { Navbar, Jumbotron, Button } from 'react-bootstrap'
```

Теперь вы готовы использовать импортированные компоненты React Bootstrap в вашей иерархии компонентов, определенной в методе render. Вот пример [`App.js`](https://gist.githubusercontent.com/gaearon/85d8c067f6af1e56277c82d19fd4da7b/raw/6158dd991b67284e9fc8d70b9d973efe87659d72/App.js) переделано с использованием React Bootstrap.

### Использование пользовательской темы

Иногда вам может потребоваться изменить визуальные стили Bootstrap (или аналогичного пакета).
Мы предлагаем следующий подход:

- Создайте новый пакет, который зависит от того, какой пакет вы хотите настроить, например Bootstrap.
- Добавьте необходимые шаги сборки, чтобы настроить тему, и опубликуйте свой пакет в npm.
- Установите свой собственный пакет npm для темы в качестве зависимости от вашего приложения.

Вот пример добавления [настраиваемого загрузчика](https://medium.com/@tacomanator/customizing-create-react-app-aa9ffb88165), который выполняется следующим образом.

## Добавление потока

Flow - это средство проверки статических типов, которое помогает вам писать код с меньшим количеством ошибок. Ознакомьтесь с этим [введение в использование статических типов в JavaScript](https://medium.com/@preethikasireddy/why-use-static-types-in-javascript-part-1-8382da1e0adb), если вы новичок в этой концепции.

Последние версии [Flow](http://flowtype.org/) работают с проектами приложений Create React "из коробки".

Чтобы добавить Flow в проект Create React App, выполните следующие действия:

1. Run `npm install --save flow-bin` (or `yarn add flow-bin`).
2. Add `"flow": "flow"` to the `scripts` section of your `package.json`.
3. Run `npm run flow init` (or `yarn flow init`) to create a [`.flowconfig` file](https://flowtype.org/docs/advanced-configuration.html) in the root directory.
4. Add `// @flow` to any files you want to type check (for example, to `src/App.js`).

Теперь вы можете запустить "npm run flow" (или "yarn flow"), чтобы проверить файлы на ошибки ввода.
При желании вы можете использовать IDE, например [Nuclide](https://nuclide.io/docs/languages/flow/), для лучшей интеграции.
В будущем мы планируем еще более тесно интегрировать его в приложение Create React.

Чтобы узнать больше о Flow, ознакомьтесь с [документацией к нему](https://flowtype.org/).

## Добавление маршрутизатора

Приложение Create React не предписывает конкретного решения для маршрутизации, но [React Router](https://react training.com/react-router/) является наиболее популярным.

Чтобы добавить его, запустите:

```sh
npm install --save react-router-dom
```

Alternatively you may use `yarn`:

```sh
yarn add react-router-dom
```

Чтобы попробовать, удалите весь код из "src/App.js" и замените его любым из примеров на веб-сайте. [Базовый пример](https://reacttraining.com/react-router/web/example/basic) - это хорошее место для начала.

Обратите внимание, что [возможно, вам потребуется настроить рабочий сервер для поддержки маршрутизации на стороне клиента] (#serving-apps-with-client-side-routing) перед развертыванием вашего приложения.

## Добавление пользовательских переменных среды

> Примечание: эта функция доступна с `react-scripts@0.2.3` и выше.

Ваш проект может использовать переменные, объявленные в вашей среде, как если бы они были объявлены локально в ваших JS-файлах. По
умолчанию для вас будет определен `NODE_ENV` и любые другие переменные среды, начинающиеся с
`REACT_APP_`.

**Переменные среды внедряются во время сборки**. Поскольку приложение Create React создает статический пакет HTML/CSS/JS, оно не может прочитать их во время выполнения. Чтобы прочитать их во время выполнения, вам нужно будет загрузить HTML-код в память на сервере и заменить заполнители во время выполнения, точно так же, как [описано здесь] (#ввод данных с сервера на страницу). В качестве альтернативы вы можете перестроить приложение на сервере в любое время, когда измените их.

> Примечание: Вы должны создать пользовательские переменные среды, начинающиеся с `REACT_APP_`. Любые другие переменные, кроме `NODE_ENV`, будут игнорироваться во избежание случайного [раскрытия закрытого ключа на компьютере, который может иметь такое же имя](https://github.com/facebookincubator/create-react-app/issues/865#issuecomment-252199527). Для изменения любых переменных среды потребуется перезапустить сервер разработки, если он запущен.

Эти переменные среды будут определены для вас в `process.env`. Например, при наличии среды
переменная с именем "REACT_APP_SECRET_CODE" будет отображаться в вашем JS как "process.env.REACT_APP_SECRET_CODE".

Существует также специальная встроенная переменная среды с именем "NODE_ENV`. Вы можете прочитать это из файла `process.env.NODE_ENV`. Когда вы запускаете `npm start", оно всегда равно `development", когда вы запускаете `npm test", оно всегда равно "test", а когда вы запускаете "npm run build" для создания производственного пакета, оно всегда равно "production". ** Вы не можете переопределить `NODE_ENV` вручную.** Это предотвращает случайное развертывание разработчиками медленной сборки для разработки в рабочей среде.

Эти переменные среды могут быть полезны для условного отображения информации в зависимости от того, где
развернут проект, или для использования конфиденциальных данных, которые находятся за пределами системы управления версиями.

Во-первых, вам необходимо определить переменные среды. Например, предположим, вы хотите использовать секрет, определенный
в среде внутри `<формы>`:

```jsx
render() {
  return (
    <div>
      <small>You are running this application in <b>{process.env.NODE_ENV}</b> mode.</small>
      <form>
        <input type="hidden" defaultValue={process.env.REACT_APP_SECRET_CODE} />
      </form>
    </div>
  );
}
```

Во время сборки `process.env.REACT_APP_SECRET_CODE` будет заменен текущим значением переменной окружения `REACT_APP_SECRET_CODE`. Помните, что переменная `NODE_ENV` будет установлена для вас автоматически.

Когда вы загрузите приложение в браузере и проверите "<ввод>", вы увидите, что для него установлено значение "abcdef", а жирным шрифтом выделена среда, предоставляемая при использовании `npm start`:

```html
<div>
	<small>You are running this application in <b>development</b> mode.</small>
	<form>
		<input type="hidden" value="abcdef" />
	</form>
</div>
```

Приведенная выше форма ищет переменную с именем `REACT_APP_SECRET_CODE` из среды. Чтобы использовать это
значение, нам нужно, чтобы оно было определено в среде. Это можно сделать двумя способами: либо в вашей командной строке, либо в
файле `.env`. Оба этих способа описаны в следующих нескольких разделах.

Наличие доступа к `NODE_ENV` также полезно для условного выполнения действий:

```js
if (process.env.NODE_ENV !== 'production') {
	analytics.disable()
}
```

Когда вы компилируете приложение с помощью "npm run build", на этапе минимизации это условие будет устранено, и результирующий пакет будет меньше.

### Ссылки на переменные среды в HTML

> Примечание: эта функция доступна с помощью `react-scripts@0.9.0" и более поздних версий.

Вы также можете получить доступ к переменным среды, начинающимся с `REACT_APP_` в `public/index.html`. Например:

```html
<title>%REACT_APP_WEBSITE_NAME%</title>
```

Обратите внимание, что применяются предостережения из приведенного выше раздела:

- Для работы, за исключением нескольких встроенных переменных (`NODE_ENV` и `PUBLIC_URL`), имена переменных должны начинаться с `REACT_APP_`.
- Переменные среды вводятся во время сборки. Если вам нужно ввести их во время выполнения, [вместо этого используйте этот подход] (#генерирование динамических мета-тегов на сервере).

### Добавление временных переменных среды в вашу командную строку

Определение переменных среды может варьироваться в зависимости от операционной системы. Также важно знать, что этот способ является временным на весь
срок действия сеанса shell.

#### Windows (cmd.exe)

```cmd
set "REACT_APP_SECRET_CODE=abcdef" && npm start
```

(Примечание: Кавычки вокруг присвоения переменной необходимы, чтобы избежать пробелов в конце.)

#### Windows (Powershell)

```Powershell
($env:REACT_APP_SECRET_CODE = "abcdef") -and (npm start)
```

#### Linux, macOS (Bash)

```bash
REACT_APP_SECRET_CODE=abcdef npm start
```

### Добавление переменных среды разработки в `.env`

> Примечание: эта функция доступна в `react-scripts@0.5.0` и более поздних версиях.

Чтобы определить постоянные переменные среды, создайте файл с именем `.env" в корне вашего проекта.:

```
REACT_APP_SECRET_CODE=abcdef
```

> Примечание: Вы должны создать пользовательские переменные среды, начинающиеся с `REACT_APP_`. Любые другие переменные, кроме `NODE_ENV`, будут игнорироваться во избежание [случайного раскрытия закрытого ключа на компьютере, который может иметь такое же имя](https://github.com/facebookincubator/create-react-app/issues/865#issuecomment-252199527). Изменение любых переменных среды потребует от вас перезапуска сервера разработки, если он запущен.

Файлы `.env` ** должны быть ** возвращены в систему управления версиями (за исключением файлов `.env*.local`).

#### Какие еще файлы `.env` можно использовать?

> Примечание: эта функция ** доступна для `react-scripts@1.0.0` и более поздних версий **.

- `.env`: По умолчанию.
- `.env.local`: Локальные переопределения. **Этот файл загружается для всех сред, кроме тестовой.**
- `.env.development`, `.env.test`, `.env.production`: настройки, зависящие от среды.
- `.env.development.local`, ".env.test.local", ".env.production.локальный`: Локальные переопределения параметров, зависящих от среды.

Файлы слева имеют больший приоритет, чем файлы справа:

- `запуск npm": ".env.development.local", ".env.development`, `.env.local`, `.env`
- `npm запускает сборку`: `.env.production.локальный`, `.env.production`, `.env.local`, `.env`
- `тест npm": ".env.test.local", ".env.test", ".env" (обратите внимание, что ".env.local" отсутствует)

Эти переменные будут использоваться по умолчанию, если компьютер не установит их явно.
Пожалуйста, обратитесь к документации [dotenv](https://github.com/motdotla/dotenv) для получения более подробной информации.

> Примечание: Если вы определяете переменные среды для разработки, вашей платформе CI и/или хостинга, скорее всего, потребуется
> они также определены. Обратитесь к их документации, как это сделать. Например, смотрите документацию для [Travis CI](https://docs.travis-ci.com/user/environment-variables/) или [Heroku](https://devcenter.heroku.com/articles/config-vars).

#### Расширение переменных среды в `.env`

> Примечание: эта функция доступна в версиях `react-scripts@1.1.0` и выше.

Расширьте переменные, которые уже установлены на вашем компьютере, для использования в вашем файле `.env` (используя [dotenv-expand](https://github.com/motdotla/dotenv-expand)).

Например, чтобы получить переменную окружения `npm_package_version`:

```
REACT_APP_VERSION=$npm_package_version
# also works:
# REACT_APP_VERSION=${npm_package_version}
```

Или разверните переменные, локальные для текущего файла `.env`:

```
DOMAIN=www.example.com
REACT_APP_FOO=$DOMAIN/foo
REACT_APP_BAR=$DOMAIN/bar
```

## Могу ли я использовать декораторы?

Многие популярные библиотеки используют [decorators](https://medium.com/google-developers/exploring-es7-decorators-76ecb65fb841) в своей документации.
На данный момент приложение Create React не поддерживает синтаксис декоратора, потому что:

- Это экспериментальное предложение, и оно может быть изменено.
- Текущая версия спецификации официально не поддерживается Babel.
- Если спецификация изменится, мы не сможем написать кодовую модификацию, потому что мы не используем ее внутри Facebook.

Однако во многих случаях вы можете переписать код на основе декоратора без использования декораторов.
Пожалуйста, обратитесь к этим двум темам для справки:

- [#214](https://github.com/facebookincubator/create-react-app/issues/214)
- [#411](https://github.com/facebookincubator/create-react-app/issues/411)

Приложение Create React добавит поддержку декоратора, когда спецификация выйдет на стабильную стадию.

## Выборка данных с помощью AJAX-запросов

React не предписывает конкретного подхода к выборке данных, но люди обычно используют либо библиотеки, подобные [axios](https://github.com/axios/axios), либо API [`fetch()`](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API), предоставляемые браузером. Удобно, что приложение Create React включает в себя функцию polyfill для `fetch()`, так что вы можете использовать его, не беспокоясь о поддержке браузера.

Глобальная функция "fetch" позволяет легко выполнять AJAX-запросы. Она принимает URL-адрес в качестве входных данных и возвращает "Promise", который преобразуется в объект "Response". Вы можете найти более подробную информацию о `fetch` [здесь](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch).

Этот проект также включает в себя [Promise polyfill](https://github.com/then/promise), который обеспечивает полную реализацию Promises/A+. Обещание представляет собой конечный результат асинхронной операции, вы можете найти более подробную информацию о Promises [здесь](https://www.promisejs.org/) и [здесь](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise). И axios, и `fetch()` используют Promises в скрытом виде. Вы также можете использовать синтаксис [`async / await`](https://davidwalsh.name/async-await), чтобы уменьшить вложенность обратного вызова.

Вы можете узнать больше о выполнении AJAX-запросов из компонентов React в [разделе часто задаваемых вопросов на веб-сайте React](https://reactjs.org/docs/faq-ajax.html).

## Интеграция с серверной частью API

Эти руководства помогут вам интегрировать ваше приложение с серверной частью API, работающей на другом порту,
используя для доступа к ней функцию `fetch()`.

### Node

Ознакомьтесь с [этим руководством](https://www.fullstackreact.com/articles/using-create-react-app-with-a-server/).
Вы можете найти сопутствующий репозиторий GitHub [здесь](https://github.com/fullstackreact/food-lookup-demo).

### Ruby на рельсах

Ознакомьтесь с [этим tutorial](https://www.fullstackreact.com/articles/how-to-get-create-react-app-to-work-with-your-rails-api/).
Вы можете найти сопутствующий репозиторий на GitHub [здесь](https://github.com/fullstackreact/food-lookup-demo-rails).

## Проксирование запросов API в процессе разработки

> Примечание: эта функция доступна с `react-scripts@0.2.3` и выше.

Пользователи часто используют интерфейсное приложение React с того же хоста и порта, что и их серверная реализация.<br>
Например, после развертывания приложения производственная настройка может выглядеть следующим образом:

```
/             - static server returns index.html with React app
/todos        - static server returns index.html with React app
/api/todos    - server handles any /api/* requests using the backend implementation
```

Такая настройка не требуется. Однако, если у вас есть такая настройка, удобно писать запросы типа `fetch('/api/todos')`, не беспокоясь о перенаправлении их на другой хост или порт во время разработки.

Чтобы указать серверу разработки перенаправлять любые неизвестные запросы на ваш API-сервер в процессе разработки, добавьте поле "прокси" в свой "package.json", например:

```js
  "proxy": "http://localhost:4000",
```

Таким образом, когда вы "извлекаете("/api/todos")" в процессе разработки, сервер разработки распознает, что это не статический ресурс, и перенаправит ваш запрос на "http://localhost:4000/api/todos" в качестве запасного варианта. Сервер разработки будет пытаться отправлять прокси-серверу запросы без "text/html" в заголовке "Accept".

Что удобно, это позволяет избежать [CORS issues](http://stackoverflow.com/questions/21854516/understanding-ajax-cors-and-security-considerations) и сообщений об ошибках, подобных этому, при разработке.:

```
Fetch API cannot load http://localhost:4000/api/todos. No 'Access-Control-Allow-Origin' header is present on the requested resource. Origin 'http://localhost:3000' is therefore not allowed access. If an opaque response serves your needs, set the request's mode to 'no-cors' to fetch the resource with CORS disabled.
```

Имейте в виду, что "прокси" действует только в процессе разработки (с "запуском npm"), и вы должны убедиться, что URL-адреса, подобные "/api/todos", указывают на нужные объекты в рабочей среде. Вам не обязательно использовать префикс "/api". Любой нераспознанный запрос без заголовка `text/html` accept будет перенаправлен на указанный "прокси".

Опция `прокси` поддерживает соединения HTTP, HTTPS и WebSocket.<br>
Если опция "прокси" для вас недостаточно гибкая, вы можете воспользоваться альтернативой:

- [Настроить прокси самостоятельно](#настройка прокси-сервера вручную).
- Включите CORS на вашем сервере ([вот как это сделать для Express](http://enable-cors.org/server_expressjs.html)).
- Используйте [переменные среды] (#добавление пользовательских переменных среды), чтобы внедрить в ваше приложение правильный серверный узел и порт.

### Ошибки "Недопустимый заголовок Узла" После Настройки Прокси-Сервера

Когда вы включаете опцию "прокси", вы соглашаетесь на более строгий набор проверок хостов. Это необходимо, поскольку, оставляя серверную часть открытой для удаленных хостов, ваш компьютер становится уязвимым для атак с повторной привязкой DNS. Проблема описана в [этой статье](https://medium.com/webpack/webpack-dev-server-middleware-security-issues-1489d950874a) и [в этом выпуске](https://github.com/webpack/webpack-dev-server/issues/887).

Это не должно повлиять на вас при разработке на "локальном хостинге", но если вы разрабатываете удаленно, как [описано здесь](https://github.com/facebookincubator/create-react-app/issues/2271), вы увидите эту ошибку в браузере после включения опции `прокси`:

> Недопустимый заголовок хоста

Чтобы обойти это, вы можете указать свой общедоступный хост разработки в файле с именем ".env.development" в корне вашего проекта:

```
HOST=mypublicdevhost.com
```

Если вы сейчас перезапустите сервер разработки и загрузите приложение с указанного хоста, оно должно сработать.

Если у вас все еще возникают проблемы или вы используете более экзотическую среду, например облачный редактор, вы можете полностью обойти проверку хоста, добавив строку в ".env.development.local". **Обратите внимание, что это опасно и подвергает ваш компьютер удаленному выполнению кода с вредоносных веб-сайтов.:**

```
# NOTE: THIS IS DANGEROUS!
# It exposes your machine to attacks from the websites you visit.
DANGEROUSLY_DISABLE_HOST_CHECK=true
```

Мы не рекомендуем такой подход.

### Настройка прокси-сервера вручную

> Примечание: эта функция доступна с параметром "react-scripts@1.0.0` и выше.

Если параметр `прокси` недостаточно гибок для вас, вы можете указать объект в следующей форме (в файле "package.json`).<br>
Вы также можете указать любое поддерживаемое значение конфигурации [`http-proxy-middleware`](https://github.com/chimurai/http-proxy-middleware#options) или [`http-proxy`](https://github.com/nodejitsu/node-http-proxy#options).

```js
{
  // ...
  "proxy": {
    "/api": {
      "target": "<url>",
      "ws": true
      // ...
    }
  }
  // ...
}
```

Все запросы, соответствующие этому пути, будут прокси-серверами, без каких-либо исключений. Сюда входят запросы для "text/html", которые не прокси-серверируются стандартным параметром "proxy".

Если вам нужно указать несколько прокси-серверов, вы можете сделать это, указав дополнительные записи.
Совпадения - это регулярные выражения, так что вы можете использовать регулярное выражение для сопоставления нескольких путей.

```js
{
  // ...
  "proxy": {
    // Matches any request starting with /api
    "/api": {
      "target": "<url_1>",
      "ws": true
      // ...
    },
    // Matches any request starting with /foo
    "/foo": {
      "target": "<url_2>",
      "ssl": true,
      "pathRewrite": {
        "^/foo": "/foo/beta"
      }
      // ...
    },
    // Matches /bar/abc.html but not /bar/sub/def.html
    "/bar/[^/]*[.]html": {
      "target": "<url_3>",
      // ...
    },
    // Matches /baz/abc.html and /baz/sub/def.html
    "/baz/.*/.*[.]html": {
      "target": "<url_4>"
      // ...
    }
  }
  // ...
}
```

### Настройка прокси-сервера WebSocket

При настройке прокси-сервера WebSocket необходимо учитывать некоторые дополнительные соображения.

Если вы используете движок WebSocket, такой как [Socket.io](https://socket.io/), у вас должен быть сокет.запущен сервер ввода-вывода, который вы можете использовать в качестве целевого прокси-сервера. Разъем.ввод-вывод не будет работать со стандартным сервером WebSocket. В частности, не ожидайте, что Socket.ввод-вывод будет работать с [тестом websocket.org echo](http://websocket.org/echo.html).

Есть хорошая документация по [настройке сокета.сервер ввода-вывода](https://socket.io/docs/).

Стандартные WebSockets ** будут ** работать как со стандартным сервером WebSocket, так и с websocket.org эхо-тест. Вы можете использовать такие библиотеки, как [ws](https://github.com/websockets/ws) для сервера с помощью [встроенных веб-сокетов в браузере](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket).

В любом случае, вы можете проксировать запросы WebSocket вручную в "package.json`:

```js
{
  // ...
  "proxy": {
    "/socket": {
      // Your compatible WebSocket server
      "target": "ws://<socket_url>",
      // Tell http-proxy-middleware that this is a WebSocket proxy.
      // Also allows you to proxy WebSocket requests without an additional HTTP request
      // https://github.com/chimurai/http-proxy-middleware#external-websocket-upgrade
      "ws": true
      // ...
    }
  }
  // ...
}
```

## Использование HTTPS при разработке

> Примечание: эта функция доступна с `react-scripts@0.4.0` и выше.

Возможно, вам потребуется, чтобы сервер разработки обслуживал страницы по протоколу HTTPS. Один из конкретных случаев, когда это может быть полезно, - это использование [функции "прокси"] (#proxying-api-requests-in-development) для прокси-запросов к API-серверу, когда этот API-сервер сам обслуживает HTTPS.

Чтобы сделать это, установите для переменной окружения "HTTPS" значение "true", затем запустите сервер разработки как обычно с помощью "npm start`:

#### Windows (cmd.exe)

```cmd
set HTTPS=true&&npm start
```

#### Windows (Powershell)

```Powershell
($env:HTTPS = $true) -and (npm start)
```

(Note: the lack of whitespace is intentional.)

#### Linux, macOS (Bash)

```bash
HTTPS=true npm start
```

Обратите внимание, что сервер будет использовать самозаверяющий сертификат, поэтому ваш веб-браузер почти наверняка выдаст предупреждение при доступе к странице.

## Генерирование динамических тегов "<meta>" Теги на сервере

Поскольку приложение Create React не поддерживает серверный рендеринг, вам может быть интересно, как сделать теги "<meta>" динамическими и отражающими текущий URL. Чтобы решить эту проблему, мы рекомендуем добавить заполнители в HTML, например, так:

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta property="og:title" content="__OG_TITLE__" />
		<meta property="og:description" content="__OG_DESCRIPTION__" />
	</head>
</html>
```

Затем на сервере, независимо от используемого вами бэкенда, вы можете записать "index.html" в память и заменить `__OG_TITLE__`, `__OG_DESCRIPTION__` и любые другие заполнители значениями, зависящими от текущего URL. Просто убедитесь, что интерполированные значения обработаны и экранированы, чтобы их можно было безопасно вставлять в HTML!

Если вы используете сервер Node, вы даже можете совместно использовать логику сопоставления маршрутов между клиентом и сервером. Однако дублирование также отлично работает в простых случаях.

## Предварительный рендеринг в статические HTML-файлы

Если вы размещаете свою "сборку" у поставщика статического хостинга, вы можете использовать [react-snapshot](https://www.npmjs.com/package/react-snapshot) или [react-snapshot](https://github.com/stereobooster/react-snap) для создания HTML-страниц для каждого маршрута или относительной ссылки в вашем приложении. Затем эти страницы будут автоматически активированы, или “увлажнены”, после загрузки пакета JavaScript.

Также есть возможности использовать это за пределами статического хостинга, чтобы снизить нагрузку на сервер при генерации и кэшировании маршрутов.

Основное преимущество предварительного рендеринга заключается в том, что вы получаете основное содержимое каждой страницы с полезной нагрузкой HTML - независимо от того, успешно ли загружен ваш пакет JavaScript. Это также увеличивает вероятность того, что поисковые системы будут отслеживать каждый маршрут вашего приложения.

Вы можете прочитать больше о [предварительном рендеринге с нулевой настройкой (также называемом моментальным снимком) здесь](https://medium.com/superhighfives/an-almost-static-stack-6df0a2791319).

## Ввод данных с сервера на страницу

Аналогично предыдущему разделу, вы можете оставить в HTML некоторые заполнители, которые вводят глобальные переменные, например:

```js
<!doctype html>
<html lang="en">
  <head>
    <script>
      window.SERVER_DATA = __SERVER_DATA__;
    </script>
```

Затем, на сервере, вы можете заменить "**SERVER_DATA**" на JSON-файл с реальными данными непосредственно перед отправкой ответа. Затем клиентский код может прочитать "window.SERVER_DATA", чтобы использовать его. ** Обязательно [очистите JSON-файл перед отправкой в client](https://medium.com/node-security/the-most-common-xss-vulnerability-in-react-js-applications-2bdffbcc1fa0), так как это делает ваше приложение уязвимым для XSS-атак.**

## Запуск тестов

> Примечание: эта функция доступна с "react-scripts@0.3.0` и выше.<br> >[Прочитайте руководство по миграции, чтобы узнать, как включить ее в старых проектах!](https://github.com/facebookincubator/create-react-app/blob/master/CHANGELOG.md#migrating-from-023-to-030)

Приложение Create React использует [Jest](https://facebook.github.io/jest/) в качестве средства запуска тестирования. Чтобы подготовиться к этой интеграции, мы провели [серьезную переработку] (https://facebook.github.io/jest/blog/2016/09/01/jest-15.html) Jest, так что, если вы слышали о нем плохие отзывы много лет назад, попробуйте еще раз.

Jest запускается на основе Node. Это означает, что тесты всегда выполняются в среде Node, а не в реальном браузере. Это позволяет нам увеличить скорость итераций и избежать сбоев.

В то время как Jest предоставляет глобальные настройки браузера, такие как "window", благодаря [jsdom](https://github.com/tmpvar/jsdom), они являются лишь приблизительным отображением реального поведения браузера. Jest предназначен для модульного тестирования вашей логики и ваших компонентов, а не для использования в DOM.

Мы рекомендуем вам использовать отдельный инструмент для сквозных тестов браузера, если они вам нужны. Они выходят за рамки Create React App.

### Соглашения об именах файлов

Jest будет искать тестовые файлы с любым из следующих популярных соглашений об именах:

- Файлы с суффиксом ".js" в папках "**tests**".
- Файлы с суффиксом ".test.js.
- Файлы с суффиксом ".spec.js`.

Файлы `.test.js` / `.spec.js" (или папки "**tests**") могут быть расположены на любой глубине в папке верхнего уровня "src".

Мы рекомендуем размещать тестовые файлы (или папки `__tests__`) рядом с тестируемым кодом, чтобы относительный импорт был короче. Например, если "App.test.js`и`App.js" находятся в одной и той же папке, для теста просто нужно "импортировать приложение из "./App" вместо длинного относительного пути. Расположение по умолчанию также помогает быстрее находить тесты в крупных проектах.

### Интерфейс командной строки

Когда вы запускаете "npm test", Jest запускается в режиме просмотра. Каждый раз, когда вы сохраняете файл, он повторно запускает тесты, точно так же, как "npm start" перекомпилирует код.

Программа watcher включает в себя интерактивный интерфейс командной строки, позволяющий запускать все тесты или ориентироваться на шаблон поиска. Она разработана таким образом, чтобы вы могли держать ее открытой и наслаждаться быстрым повторным запуском. Вы можете ознакомиться с командами в разделе “Использование Watch”. Обратите внимание, что программа watcher печатает после каждого запуска:

![Простой режим просмотра](http://facebook.github.io/jest/img/blog/15-watch.gif)

### Интеграция с системой контроля версий

По умолчанию, когда вы запускаете "npm-тест", Jest запускает только тесты, относящиеся к файлам, измененным с момента последней фиксации. Это оптимизация, разработанная для того, чтобы ваши тесты выполнялись быстро, независимо от того, сколько у вас тестов. Однако предполагается, что вы не часто фиксируете код, который не проходит тесты.

В Jest всегда будет явно указано, что он запускал тесты, относящиеся только к файлам, измененным с момента последней фиксации. Вы также можете нажать "a" в режиме просмотра, чтобы заставить Jest выполнить все тесты.

Jest всегда будет запускать все тесты на сервере [непрерывной интеграции] (#continuous-integration) или если проект не находится в репозитории Git или Mercurial.

### Написание тестов

Чтобы создать тесты, добавьте блоки "it()" (или "test()") с названием теста и его кодом. При желании вы можете обернуть их в блоки "describe()" для логической группировки, но это не обязательно и не рекомендуется.

Jest предоставляет встроенную глобальную функцию expect() для создания утверждений. Базовый тест может выглядеть следующим образом:

```js
import sum from './sum'

it('sums numbers', () => {
	expect(sum(1, 2)).toEqual(3)
	expect(sum(2, 2)).toEqual(4)
})
```

Все средства сопоставления `expect()`, поддерживаемые Just, [подробно описаны здесь](https://facebook.github.io/jest/docs/en/expect.html#content).<br>
Вы также можете использовать [`jest.fn()` и `expect(fn).toBeCalled()`](https://facebook.github.io/jest/docs/en/expect.html#tohavebeencalled) для создания “шпионских” или имитационных функций.

### Тестирование компонентов

Существует широкий спектр методов тестирования компонентов. Они варьируются от “дымового теста”, проверяющего, что компонент отрисовывается без сбоев, до поверхностного рендеринга и тестирования части выходных данных, а также полного рендеринга и тестирования жизненного цикла компонента и изменений состояния.

В разных проектах используются разные подходы к тестированию в зависимости от того, как часто меняются компоненты и какой объем логики они содержат. Если вы еще не определились со стратегией тестирования, мы рекомендуем начать с создания простых smoke-тестов для ваших компонентов:

```js
import React from 'react'
import ReactDOM from 'react-dom'
import App from './App'

it('renders without crashing', () => {
	const div = document.createElement('div')
	ReactDOM.render(<App />, div)
})
```

Этот тест монтирует компонент и проверяет, не произошел ли сбой в его работе во время рендеринга. Тесты, подобные этому, приносят большую пользу при минимальных усилиях, поэтому они хороши в качестве отправной точки, и именно этот тест вы найдете в разделе `src/App.test.js`.

Когда вы столкнетесь с ошибками, вызванными изменением компонентов, вы получите более глубокое представление о том, какие из них стоит протестировать в вашем приложении. Возможно, сейчас самое подходящее время представить более конкретные тесты, подтверждающие конкретные ожидаемые результаты или поведение.

Если вы хотите протестировать компоненты отдельно от дочерних компонентов, которые они отображают, мы рекомендуем использовать [`shallow()` rendering API](http://airbnb.io/enzyme/docs/api/shallow.html) из [Enzyme](http://airbnb.io/enzyme/). Чтобы установить его, запустите:

```sh
npm install --save enzyme enzyme-adapter-react-16 react-test-renderer
```

В качестве альтернативы вы можете использовать `yarn`:

```sh
yarn add enzyme enzyme-adapter-react-16 react-test-renderer
```

Начиная с Enzyme 3, вам нужно будет установить Enzyme вместе с адаптером, соответствующим используемой вами версии React. (В приведенных выше примерах используется адаптер для React 16.)

Адаптер также необходимо будет настроить в вашем [глобальном установочном файле] (#initializing-test-environment).:

#### `src/setupTests.js`

```js
import { configure } from 'enzyme'
import Adapter from 'enzyme-adapter-react-16'

configure({ adapter: new Adapter() })
```

> Примечание: Имейте в виду, что если вы решите "удалить" перед созданием "src/setupTests.js", результирующий файл "package.json" не будет содержать никаких ссылок на него. [Прочитайте здесь](#initializing-test-environment), чтобы узнать, как добавить это после извлечения.

Теперь вы можете написать тест на курение с его помощью:

```js
import React from 'react'
import { shallow } from 'enzyme'
import App from './App'

it('renders without crashing', () => {
	shallow(<App />)
})
```

В отличие от предыдущего теста smoke с использованием "ReactDOM.render()", этот тест отображает только "<Приложение>" и не углубляется. Например, даже если "<Приложение>" само отображает "<Кнопку>", которая запускается, этот тест будет пройден. Поверхностный рендеринг отлично подходит для изолированных модульных тестов, но вы все равно можете захотеть создать несколько полноценных тестов рендеринга, чтобы убедиться в правильной интеграции компонентов. Enzyme поддерживает [полный рендеринг с помощью `mount()`](http://airbnb.io/enzyme/docs/api/mount.html), и вы также можете использовать его для тестирования изменений состояния и жизненного цикла компонентов.

Вы можете прочитать [Документацию по ферментам](http://airbnb.io/enzyme/) для получения дополнительной информации о методах тестирования. В документации по ферментам используются Chai и Sinon для утверждений, но вам не обязательно их использовать, поскольку Jest предоставляет встроенные функции `expect()` и `jest.fn()` для шпионов.

Вот пример из документации Enzyme, который утверждает конкретные выходные данные, переписанные для использования Jest matchers:

```js
import React from 'react'
import { shallow } from 'enzyme'
import App from './App'

it('renders welcome message', () => {
	const wrapper = shallow(<App />)
	const welcome = <h2>Welcome to React</h2>
	// expect(wrapper.contains(welcome)).to.equal(true);
	expect(wrapper.contains(welcome)).toEqual(true)
})
```

Все средства сопоставления Jest [подробно описаны здесь] (http://facebook.github.io/jest/docs/en/expect.html).
Тем не менее, вы можете использовать стороннюю библиотеку утверждений, такую как [Chai] (http://chaijs.com/), если хотите, как описано ниже.

Кроме того, вы можете найти [jest-enzyme](https://github.com/blainekasten/enzyme-matchers) полезным для упрощения ваших тестов с помощью удобочитаемых средств сопоставления. Приведенный выше код "contains" может быть написан более просто с помощью jest-enzyme.

```js
expect(wrapper).toContainReact(welcome)
```

To enable this, install `jest-enzyme`:

```sh
npm install --save jest-enzyme
```

Alternatively you may use `yarn`:

```sh
yarn add jest-enzyme
```

Import it in [`src/setupTests.js`](#initializing-test-environment) to make its matchers available in every test:

```js
import 'jest-enzyme'
```

### Использование сторонних библиотек утверждений

Мы рекомендуем использовать `expect()` для утверждений и `jest.fn()` для шпионов. Если у вас возникли проблемы с ними, пожалуйста, [отметьте их в Jest](https://github.com/facebook/jest/issues/new), и мы их исправим. Мы намерены продолжать улучшать их для React, поддерживая, например, [красивую печать элементов React в формате JSX](https://github.com/facebook/jest/pull/1566).

Однако, если вы привыкли к другим библиотекам, таким как [Chai](http://chaijs.com/) и [Sinon](http://sinonjs.org/), или если у вас есть существующий код, использующий их, который вы хотели бы перенести, вы можете импортировать их обычным способом следующим образом:

```js
import sinon from 'sinon'
import { expect } from 'chai'
```

а затем используйте их в своих тестах, как обычно.

### Инициализация тестовой среды

> Примечание: эта функция доступна с `react-scripts@0.4.0" и выше.

Если ваше приложение использует API браузера, который вам нужно имитировать в тестах, или если вам просто нужна глобальная настройка перед запуском тестов, добавьте в свой проект символ "src/setupTests.js`. Он будет автоматически выполнен перед запуском тестов.

Например:

#### `src/setupTests.js`

```js
const localStorageMock = {
	getItem: jest.fn(),
	setItem: jest.fn(),
	clear: jest.fn(),
}
global.localStorage = localStorageMock
```

> Примечание: Имейте в виду, что если вы решите "извлечь" перед созданием `src/setupTests.js `, результирующий файл "package.json" не будет содержать никаких ссылок на него, поэтому вам следует вручную создать свойство "setupTestFrameworkScriptFile" в конфигурации для Jest, что-то вроде следующего:

> ```js
> "jest": {
>   // ...
>   "setupTestFrameworkScriptFile": "<rootDir>/src/setupTests.js"
>  }
> ```

### Фокусировка и исключение тестов

Вы можете заменить "it()" на "it()", чтобы временно исключить выполнение теста.<br>
Аналогично, "fit()" позволяет сосредоточиться на конкретном тесте, не выполняя никаких других тестов.

### Coverage Reporting

В Jest встроен coverage reporter, который хорошо работает с ES6 и не требует настройки.<br>
Запустите `npm test -- --coverage` (обратите внимание на дополнительный `--` в середине) чтобы включить отчет о покрытии, подобный этому:

![coverage report](http://i.imgur.com/5bFhnTS.png)

Обратите внимание, что тесты с покрытием выполняются намного медленнее, поэтому рекомендуется запускать их отдельно от обычного рабочего процесса.

#### Конфигурация

Конфигурация покрытия Jest по умолчанию может быть изменена путем добавления любого из следующих поддерживаемых ключей в конфигурацию Jest в вашем package.json.

Поддерживаемые переопределения:

- [`collectCoverageFrom`](https://facebook.github.io/jest/docs/en/configuration.html#collectcoveragefrom-array)
- [`coverageReporters`](https://facebook.github.io/jest/docs/en/configuration.html#coveragereporters-array-string)
- [`coverageThreshold`](https://facebook.github.io/jest/docs/en/configuration.html#coveragethreshold-object)
- [`snapshotSerializers`](https://facebook.github.io/jest/docs/en/configuration.html#snapshotserializers-array-string)

Пример package.json:

```json
{
	"name": "your-package",
	"jest": {
		"collectCoverageFrom": [
			"src/**/*.{js,jsx}",
			"!<rootDir>/node_modules/",
			"!<rootDir>/path/to/dir/"
		],
		"coverageThreshold": {
			"global": {
				"branches": 90,
				"functions": 90,
				"lines": 90,
				"statements": 90
			}
		},
		"coverageReporters": ["text"],
		"snapshotSerializers": ["my-serializer-module"]
	}
}
```

### Непрерывная интеграция

По умолчанию `npm test` запускает программу watcher с интерактивным интерфейсом командной строки. Однако вы можете принудительно запустить тесты один раз и завершить процесс, установив переменную среды с именем `CI`.

При создании сборки вашего приложения с помощью "npm run build" предупреждения о линтере по умолчанию не проверяются. Как и в случае с "npm test", вы можете принудительно выполнить проверку предупреждений о линтере, установив переменную окружения "CI". Если возникают какие-либо предупреждения, то сборка завершается ошибкой.

Популярные серверы CI уже установили переменную среды "CI" по умолчанию, но вы также можете сделать это самостоятельно:

### На серверах CI

#### Travis CI

1. Следуйте руководству [Начало работы Travis](https://docs.travis-ci.com/user/getting-started/) по синхронизации вашего репозитория GitHub с Travis. Возможно, вам потребуется вручную инициализировать некоторые настройки на странице [профиль](https://travis-ci.org/profile).
2. Добавьте файл `.travis.yml` в свой репозиторий git.

```
language: node_js
node_js:
  - 6
cache:
  directories:
    - node_modules
script:
  - npm run build
  - npm test
```

3. Запустите свою первую сборку с помощью git push.
4. [При необходимости настройте сборку Travis CI](https://docs.travis-ci.com/user/customizing-the-build/).

#### CircleCI

Следуйте [этой статье](https://medium.com/@knowbody/circleci-and-zeits-now-sh-c9b7eebcd3c1), чтобы настроить CircleCI с помощью проекта Create React App.

### В вашем собственном окружении

##### Windows (cmd.exe)

```cmd
set CI=true&&npm test
```

```cmd
set CI=true&&npm run build
```

(Note: the lack of whitespace is intentional.)

##### Windows (Powershell)

```Powershell
($env:CI = $true) -and (npm test)
```

```Powershell
($env:CI = $true) -and (npm run build)
```

##### Linux, macOS (Bash)

```bash
CI=true npm test
```

```bash
CI=true npm run build
```

Команда test заставит выполнить тесты только один раз вместо запуска наблюдателя.

> Если вы часто сталкиваетесь с этим в процессе разработки, пожалуйста, [сообщите о проблеме] (https://github.com/facebookincubator/create-react-app/issues/new), чтобы рассказать нам о вашем варианте использования, потому что мы хотим сделать watcher максимально удобным и готовы изменить его работу, чтобы приспособить к большему количеству рабочих процессов.

Команда build проверит наличие предупреждений linter и завершит работу с ошибкой, если таковые будут обнаружены.

### Отключение jsdom

По умолчанию "package.json" сгенерированного проекта выглядит следующим образом:

```js
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test --env=jsdom"
```

Если вы знаете, что ни один из ваших тестов не зависит от [jsdom](https://github.com/tmpvar/jsdom), вы можете спокойно удалить `--env=jsdom`, и ваши тесты будут выполняться быстрее:

```diff
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
-   "test": "react-scripts test --env=jsdom"
+   "test": "react-scripts test"
```

Чтобы помочь вам определиться, вот список API, для которых **need jsdom**:

- Any browser globals like `window` and `document`
- [`ReactDOM.render()`](https://facebook.github.io/react/docs/top-level-api.html#reactdom.render)
- [`TestUtils.renderIntoDocument()`](https://facebook.github.io/react/docs/test-utils.html#renderintodocument) ([a shortcut](https://github.com/facebook/react/blob/34761cf9a252964abfaab6faf74d473ad95d1f21/src/test/ReactTestUtils.js#L83-L91) for the above)
- [`mount()`](http://airbnb.io/enzyme/docs/api/mount.html) in [Enzyme](http://airbnb.io/enzyme/index.html)

Напротив, **jsdom is not needed** для следующих APIs:

- [`TestUtils.createRenderer()`](https://facebook.github.io/react/docs/test-utils.html#shallow-rendering) (shallow rendering)
- [`shallow()`](http://airbnb.io/enzyme/docs/api/shallow.html) in [Enzyme](http://airbnb.io/enzyme/index.html)

Finally, jsdom is also not needed for [snapshot testing](http://facebook.github.io/jest/blog/2016/07/27/jest-14.html).

### Тестирование моментальных снимков

Тестирование моментальных снимков - это функция Jest, которая автоматически создает текстовые снимки ваших компонентов и сохраняет их на диске, поэтому, если выходные данные пользовательского интерфейса изменятся, вы получите уведомление без необходимости вручную вводить какие-либо утверждения в выходные данные компонента. [Подробнее о тестировании моментальных снимков.](http://facebook.github.io/jest/blog/2016/07/27/jest-14.html)

### Интеграция с редактором

Если вы используете [Visual Studio Code](https://code.visualstudio.com), есть [расширение Jest](https://github.com/orta/vscode-jest), которое работает с приложением Create React "из коробки". Это обеспечивает множество функций, аналогичных IDE, при использовании текстового редактора: отображение статуса тестового запуска с сообщениями о возможных ошибках, автоматический запуск и остановка программы наблюдения, а также возможность обновления моментальных снимков одним щелчком мыши.

![VS Code Jest Preview](https://cloud.githubusercontent.com/assets/49038/20795349/a032308a-b7c8-11e6-9b34-7eeac781003f.png)

## Отладочные тесты

Существуют различные способы настройки отладчика для ваших Jest-тестов. Мы расскажем об отладке в Chrome и [Visual Studio Code](https://code.visualstudio.com/).

> Примечание: для отладочных тестов требуется Node 8 или более поздней версии.

### Отладочные тесты в Chrome

Добавьте следующее в раздел `скрипты` в `package.json` вашего проекта

```json
"scripts": {
    "test:debug": "react-scripts --inspect-brk test --runInBand --env=jsdom"
  }
```

Поместите инструкции `debugger;` в любой тест и запустите:

```bash
$ npm run test:debug
```

После этого запустятся ваши тесты Jest, но перед выполнением сделайте паузу, чтобы позволить отладчику подключиться к процессу.

Откройте в Chrome следующее

```
about:inspect
```

После открытия этой ссылки будут показаны инструменты разработчика Chrome. Выберите `проверять" в вашем процессе, и в первой строке скрипта react будет установлена точка останова (это сделано просто для того, чтобы дать вам время открыть инструменты разработчика и предотвратить выполнение Jest до того, как у вас будет время это сделать). Нажмите кнопку, которая выглядит как кнопка "воспроизвести" в правом верхнем углу экрана, чтобы продолжить выполнение. Когда Jest выполнит тест, содержащий инструкцию отладчика, выполнение будет приостановлено, и вы сможете проверить текущую область действия и стек вызовов.

> Примечание: параметр --runInBand cli гарантирует, что Jest запускает тесты в одном и том же процессе, а не запускает процессы для отдельных тестов. Обычно Jest распараллеливает выполнение тестов в разных процессах, но сложно отлаживать много процессов одновременно.

### Отладка тестов в Visual Studio Code

Отладка Jest-тестов поддерживается в [Visual Studio Code](https://code.visualstudio.com).

Используйте следующий конфигурационный файл [`launch.json`](https://code.visualstudio.com/docs/editor/debugging#_launch-configurations).:

```
{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Debug CRA Tests",
      "type": "node",
      "request": "launch",
      "runtimeExecutable": "${workspaceRoot}/node_modules/.bin/react-scripts",
      "args": [
        "test",
        "--runInBand",
        "--no-cache",
        "--env=jsdom"
      ],
      "cwd": "${workspaceRoot}",
      "protocol": "inspector",
      "console": "integratedTerminal",
      "internalConsoleOptions": "neverOpen"
    }
  ]
}
```

## Разработка компонентов изолированно

Обычно в приложении используется множество компонентов пользовательского интерфейса, и каждый из них имеет множество различных состояний.
Например, простой компонент кнопки может иметь следующие состояния:

- В обычном состоянии с текстовой меткой.
- В отключенном режиме.
- В состоянии загрузки.

Обычно трудно увидеть эти состояния, не запустив образец приложения или несколько примеров.

Приложение Create React по умолчанию не содержит никаких инструментов для этого, но вы можете легко добавить [Сборник рассказов для React](https://storybook.js.org) ([источник](https://github.com/storybooks/storybook)) или [Руководство по стилю React](https://react-styleguidist.js.org/) ([источник](https://github.com/styleguidist/react-styleguidist)) в свой проект. **Это сторонние инструменты, которые позволяют разрабатывать компоненты и видеть все их состояния отдельно от вашего приложения **.

![Сборник рассказов для демонстрации React](http://i.imgur.com/7CIAWpB.gif)

Вы также можете развернуть свой сборник рассказов или руководство по стилю как статическое приложение. Таким образом, все члены вашей команды смогут просматривать различные состояния компонентов пользовательского интерфейса без запуска внутреннего сервера или создания учетной записи в вашем приложении.

### Начало работы с Storybook

Storybook - это среда разработки компонентов пользовательского интерфейса React. Она позволяет просматривать библиотеку компонентов, просматривать различные состояния каждого компонента и интерактивно разрабатывать и тестировать компоненты.

Сначала установите следующий пакет npm глобально:

```sh
npm install -g @storybook/cli
```

Затем запустите следующую команду в каталоге вашего приложения:

```sh
getstorybook
```

После этого следуйте инструкциям на экране.

Узнайте больше о React Storybook:

- Screencast: [Getting Started with React Storybook](https://egghead.io/lessons/react-getting-started-with-react-storybook)
- [GitHub Repo](https://github.com/storybooks/storybook)
- [Documentation](https://storybook.js.org/basics/introduction/)
- [Snapshot Testing UI](https://github.com/storybooks/storybook/tree/master/addons/storyshots) with Storybook + addon/storyshot

### Начало работы с Styleguidist

Styleguidist сочетает в себе руководство по стилю, в котором все ваши компоненты представлены на одной странице с их реквизитами, документацией и примерами использования, и среду для изолированной разработки компонентов, аналогичную Storybook. В Styleguidist вы пишете примеры в Markdown, где каждый фрагмент кода отображается как интерактивная площадка для редактирования.

Сначала установите Styleguidist:

```sh
npm install --save react-styleguidist
```

В качестве альтернативы вы можете использовать `yarn`:

```sh
yarn add react-styleguidist
```

Затем добавьте эти скрипты в свой `package.json`:

```diff
   "scripts": {
+    "styleguide": "styleguidist server",
+    "styleguide:build": "styleguidist build",
     "start": "react-scripts start",
```

Затем запустите следующую команду в каталоге вашего приложения:

```sh
npm run styleguide
```

После этого следуйте инструкциям на экране.

Узнайте больше о React Styleguidist:

- [GitHub Repo](https://github.com/styleguidist/react-styleguidist)
- [Documentation](https://react-styleguidist.js.org/docs/getting-started.html)

## Публикация компонентов в npm

Приложение Create React не предоставляет встроенных функций для публикации компонентов в npm. Если вы готовы извлечь компонент из своего проекта, чтобы им могли пользоваться другие пользователи, мы рекомендуем переместить его в отдельный каталог за пределами вашего проекта, а затем использовать такой инструмент, как [nwb](https://github.com/insin/nwb#react-components-and-libraries), чтобы подготовить его к публикации.

## Создание прогрессивного веб-приложения

По умолчанию производственная сборка является полнофункциональной и доступна только в автономном режиме
[Прогрессивное веб-приложение](https://developers.google.com/web/progressive-web-apps/).

Прогрессивные веб-приложения работают быстрее и надежнее, чем традиционные веб-страницы, и обеспечивают привлекательный интерфейс для мобильных устройств:

- Все статические ресурсы сайта кэшируются, чтобы ваша страница быстро загружалась при последующих посещениях, независимо от подключения к сети (например, 2G или 3G). Обновления загружаются в фоновом режиме.
- Ваше приложение будет работать независимо от состояния сети, даже в автономном режиме. Это означает, что ваши пользователи смогут пользоваться вашим приложением на высоте 10 000 футов и в метро.
- На мобильных устройствах ваше приложение может быть добавлено непосредственно на главный экран пользователя, значок приложения и т.д. Вы также можете повторно привлекать пользователей с помощью веб-уведомлений **push-уведомлений **. Это устраняет необходимость в App Store.

Модуль [`sw-precache-webpack-plugin`](https://github.com/goldhand/sw-precache-webpack-plugin)
интегрирован в производственную конфигурацию
и отвечает за создание файла service worker, который автоматически
предварительно кэширует все ваши локальные ресурсы и поддерживает их в актуальном состоянии по мере развертывания обновлений.
Сотрудник службы поддержки будет использовать [сначала кэширование strategy](https://developers.google.com/web/fundamentals/instant-and-offline/offline-cookbook/#cache-falling-back-to-network)
для обработки всех запросов к локальным ресурсам, включая исходный HTML-код, гарантируя
надежную работу вашего веб-приложения даже в медленной или ненадежной сети.

### Отказ от кэширования

Если вы предпочитаете не включать service workers до первоначального
производственного развертывания, удалите вызов `registerServiceWorker()`
из [`src/index.js`](src/index.js).

Если вы ранее включили service workers в своем производственном развертывании и
решили отключить их для всех существующих пользователей,
вы можете заменить вызов на "registerServiceWorker()` в
[`src/index.js`](src/index.js) сначала путем изменения импорта сервисного работника:

```javascript
import { unregister } from './registerServiceWorker'
```

а затем вызовите вместо этого "отменить регистрацию()".
После того, как пользователь посетит страницу, на которой есть "отменить регистрацию()",
сервисный работник будет удален. Обратите внимание, что в зависимости от того, как обрабатывается `/service-worker.js`,
может потребоваться до 24 часов, чтобы кэш стал недействительным.

### Рекомендации в первую очередь в автономном режиме

1. Сервисные работники [требуют HTTPS](https://developers.google.com/web/fundamentals/getting-started/primers/service-workers#you_need_https)
   хотя для облегчения локального тестирования эта политика
   [не применяется к `localhost`](http://stackoverflow.com/questions/34160509/options-for-testing-service-workers-via-http/34161385#34161385).
   Если ваш рабочий веб-сервер не поддерживает HTTPS, то сервисный работник
   регистрация завершится неудачей, но остальная часть вашего веб-приложения останется работоспособной.

1. Сервисные работники [в настоящее время не поддерживаются] (https://jakearchibald.github.io/isserviceworkerready/)
   во всех веб-браузерах. Регистрация сервисных работников [не будет предпринята] (src/registerServiceWorker.js)
   в браузерах, которые не поддерживаются.

1. Сервисный работник включен только в [производственной среде] (#deployment),
   например, в выходных данных "npm run build`. Рекомендуется не включать
   в среду разработки сервисный центр, работающий в автономном режиме, поскольку это может привести к
   разочарованию, если будут использоваться ранее кэшированные ресурсы, не включающие последние версии.
   изменения, которые вы внесли локально.

1. Если вам необходимо протестировать свой автономный сервис worker локально, создайте
   приложение (используя "npm run build") и запустите простой http-сервер из вашего каталога сборки. После запуска сценария сборки "create-react-app" выдаст инструкции по одному из способов локального тестирования вашей производственной сборки, а в [инструкциях по развертыванию] (#deployment) есть инструкции по использованию других методов. _ Обязательно всегда используйте режим инкогнито, чтобы избежать проблем с кэшем вашего браузера._

1. Если возможно, настройте свою производственную среду для обслуживания сгенерированных
   `service-worker.js` [с HTTP-кэшированием disabled](http://stackoverflow.com/ questions/38843970/service-worker-javascript-update-frequency-every-24-hours).
   Если это невозможно — например, [GitHub Pages](#github-pages) не
   позволяет вам изменить 10—минутный срок службы HTTP-кэша по умолчанию, - то имейте в виду что если вы посетите свой рабочий сайт, а затем вернетесь к нему еще раз, прежде чем `service-worker.js` истек срок действия вашего HTTP-кэша, вы продолжите получать
   ранее кэшированные ресурсы от сервисного работника. Если у вас есть немедленная
   вам необходимо просмотреть обновленное производственное развертывание, выполнив повторное обновление временно отключит service worker и восстановит все ресурсы из сети.

1. Пользователи не всегда знакомы с веб-приложениями, работающими в автономном режиме. Может быть полезно
   [разрешить пользователю know](https://developers.google.com/web/fundamentals/instant-and-offline/offline-ux#inform_the_user_when_the_app_is_ready_for_offline_consumption)
   когда сервисный работник завершит заполнение ваших кэшей (отобразив "Этот веб-сайт
   приложение работает в автономном режиме!"), а также сообщите им, когда сотрудник службы поддержки получит последние обновления, которые будут доступны при следующей загрузке страницы (появится сообщение "Доступно новое содержимое; пожалуйста, обновите"). Показ в настоящее время это сообщение оставлено разработчику в качестве упражнения, но в качестве отправной точки вы можете использовать логику, включенную в [`src/registerServiceWorker.js`](src/registerServiceWorker.js), которая демонстрирует, какие события жизненного цикла service worker следует прослушивать для обнаружения каждого из них сценарий, и который по умолчанию просто записывает соответствующие сообщения в консоль JavaScript.

1. По умолчанию сгенерированный файл service worker не будет перехватывать или кэшировать какой-либо перекрестный трафик, такой как HTTP [запросы API] (#интеграция с серверной частью api), изображения или вставки, загруженные из другого домена. Если вы хотите использовать стратегию кэширования во время выполнения для этих запросов, вы можете [`извлечь`](#npm-run-eject) а затем настроить [`runtimeCaching`](https://github.com/GoogleChrome/sw-precache#runtimecaching-arrayobject) выберите параметр в разделе `SWPrecacheWebpackPlugin` в [`webpack.config.prod.js`](../config/webpack.config.prod.js).

### Прогрессивные метаданные веб-приложения

Конфигурация по умолчанию включает манифест веб-приложения, расположенный по адресу
[`public/manifest.json`] (общедоступный/манифест.json), который вы можете настроить с
учетом особенностей вашего веб-приложения.

Когда пользователь добавляет веб-приложение на свой рабочий стол с помощью Chrome или Firefox на
Android, метаданные в [`manifest.json`](public/manifest.json) определяют, какие
значки, названия и фирменные цвета будут использоваться при отображении веб-приложения.
[Руководство по манифесту веб-приложения](https://developers.google.com/web/fundamentals/engage-and-retain/web-app-manifest/)
предоставляет более подробную информацию о том, что означает каждое поле и как ваши настройки
повлияют на работу ваших пользователей.

## Анализ размера пакета

[Обозреватель исходных карт](https://www.npmjs.com/package/source-map-explorer) анализирует
JavaScript связывается с использованием исходных карт. Это поможет вам понять
, откуда берется избыточность кода.

Чтобы добавить обозреватель исходных карт в проект Create React App, выполните следующие действия:

```sh
npm install --save source-map-explorer
```

Alternatively you may use `yarn`:

```sh
yarn add source-map-explorer
```

Then in `package.json`, add the following line to `scripts`:

```diff
   "scripts": {
+    "analyze": "source-map-explorer build/static/js/main.*",
     "start": "react-scripts start",
     "build": "react-scripts build",
     "test": "react-scripts test --env=jsdom",
```

Затем, чтобы проанализировать пакет, запустите производственную сборку, а затем запустите сценарий анализа.

```
npm run build
npm run analyze
```

## Развертывание

`npm run build` создает каталог "build" с рабочей сборкой вашего приложения. Настройте свой любимый HTTP-сервер таким образом, чтобы посетитель вашего сайта обслуживался "index.html" и отправлял запросы по статическим путям, таким как `/static/js/main.файлы <hash>.js` передаются вместе с содержимым файла `/static/js/main.<hash>.js`.

### Статический сервер

Для сред, использующих [Node](https://nodejs.org/), самым простым способом справиться с этим было бы установить [serve](https://github.com/zeit/serve) и позволить ему обрабатывать все остальное:

```sh
npm install -g serve
serve -s build
```

Последняя команда, показанная выше, будет обслуживать ваш статический сайт через порт **5000**. Как и многие внутренние настройки [serve](https://github.com/zeit/serve), порт можно настроить с помощью флагов `-p` или `--port`.

Запустите эту команду, чтобы получить полный список доступных опций:

```sh
serve -h
```

### Другие решения

Вам не обязательно нужен статический сервер для запуска проекта Create React App в рабочей среде. Он прекрасно работает, будучи интегрированным в существующий динамический сервер.

Вот программный пример с использованием [Node](https://nodejs.org/) и [Express](http://expressjs.com/).:

```javascript
const express = require('express')
const path = require('path')
const app = express()

app.use(express.static(path.join(__dirname, 'build')))

app.get('/', function (req, res) {
	res.sendFile(path.join(__dirname, 'build', 'index.html'))
})

app.listen(9000)
```

Выбор вашего серверного программного обеспечения также не важен. Поскольку приложение Create React полностью не зависит от платформы, нет необходимости явно использовать Node.

Папка "build" со статическими ресурсами - это единственный результат, который создает приложение Create React.

Однако этого недостаточно, если вы используете маршрутизацию на стороне клиента. Прочитайте следующий раздел, если вы хотите поддерживать URL-адреса типа "/todos/42" в вашем одностраничном приложении.

### Обслуживание приложений с маршрутизацией на стороне клиента

Если вы используете маршрутизаторы, которые используют HTML5 [`pushState` history API](https://developer.mozilla.org/en-US/docs/Web/API/History_API#Adding_and_modifying_history_entries) под капотом (например, [React Router](https://github.com/ReactTraining/react-router) с `browserHistory`), многие статические файловые серверы выйдут из строя. Например, если вы использовали React Router с маршрутом для `/todos/42`, сервер разработки ответит на `localhost:3000/todos/42` должным образом, но Express, обслуживающий производственную сборку, как указано выше, не ответит.

Это происходит потому, что при загрузке новой страницы для файла "/todos/42" сервер ищет файл `build/todos/42` и не находит его. Сервер должен быть настроен таким образом, чтобы отвечать на запрос "/todos/42", отправляя "index.html`. Например, мы можем изменить наш экспресс-пример выше, чтобы он отправлял `index.html" для любых неизвестных путей:

```diff
 app.use(express.static(path.join(__dirname, 'build')));

-app.get('/', function (req, res) {
+app.get('/*', function (req, res) {
   res.sendFile(path.join(__dirname, 'build', 'index.html'));
 });
```

Если вы используете [HTTP-сервер Apache](https://httpd.apache.org/), вам необходимо создать файл ".htaccess" в папке "public", который выглядит следующим образом:

```
    Options -MultiViews
    RewriteEngine On
    RewriteCond %{REQUEST_FILENAME} !-f
    RewriteRule ^ index.html [QSA,L]
```

Он будет скопирован в папку "build", когда вы запустите "npm run build".

Если вы используете [Apache Tomcat](http://tomcat.apache.org/), вам нужно следовать [этому ответу на Stack Overflow](https://stackoverflow.com/a/41249464/4878474).

Теперь запросы к "/todos/42" будут корректно обрабатываться как в процессе разработки, так и в рабочей среде.

В рабочей сборке и в браузере, поддерживающем [service workers](https://developers.google.com/web/fundamentals/getting-started/primers/service-workers),
service worker будет автоматически обрабатывать все запросы навигации, например, для
`/todos/42`, используя кэшированную копию вашего "index.html`. Этот
навигационный маршрут service worker можно настроить или отключить с помощью
[`извлекать'](#npm-run-eject), а затем изменить параметры
[`navigateFallback`](https://github.com/GoogleChrome/sw-precache#navigatefallback-string)
и [`navigateFallbackWhitelist`](https://github.com/GoogleChrome/sw-precache#navigatefallbackwhitelist-arrayregexp)
в `SWPreachePlugin` [конфигурации](../config/webpack.config.prod.js).

Когда пользователи устанавливают ваше приложение на рабочий стол своего устройства, в конфигурации по умолчанию используется ярлык "/index.html`. Это может не сработать для маршрутизаторов на стороне клиента, которые ожидают, что приложение будет обслуживаться с помощью `/`. Отредактируйте манифест веб-приложения по адресу [`public/manifest.json`](общедоступный/манифест.json) и измените `start_url`, чтобы он соответствовал требуемой схеме URL, например:

```js
  "start_url": ".",
```

### Построение для относительных путей

По умолчанию Create React App создает сборку, предполагая, что ваше приложение размещено в корневом каталоге сервера.
Чтобы переопределить это, укажите `домашнюю страницу` в вашем `package.json`, например:

```js
  "homepage": "http://mywebsite.com/relativepath",
```

Это позволит приложению Create React правильно указать корневой путь для использования в сгенерированном HTML-файле.

**Примечание**: Если вы используете "react-router@^4", вы можете рутировать "<Link>", используя параметр "basename`на любом`<Router>`.
Дополнительная информация [здесь](https://react training.com/react-router/web/api/BrowserRouter/basename-string).<br>
<br>
Например:

```js
<BrowserRouter basename="/calendar"/>
<Link to="/today"/> // renders <a href="/calendar/today">
```

#### Использование одной и той же сборки по разным путям

> Примечание: эта функция доступна с `react-scripts@0.9.0` и выше.

Если вы не используете HTML5 pushState history API или вообще не используете маршрутизацию на стороне клиента, нет необходимости указывать URL, с которого будет отправляться ваше приложение. Вместо этого вы можете поместить это в свой `package.json`:

```js
  "homepage": ".",
```

Это позволит убедиться, что все пути к ресурсам совпадают с `index.html`. После этого вы сможете переместить свое приложение с `http://mywebsite.com` на `http://mywebsite.com/relativepath` или даже `http://mywebsite.com/relative/path" без необходимости его перестраивать.

### [Azure](https://azure.microsoft.com/)

Смотрите [это](https://medium.com/@to_pe/deploying-create-react-app-on-microsoft-azure-c0f6686a4321) сообщение в блоге о том, как развернуть ваше приложение React в Microsoft Azure.

Смотрите [это](https://medium.com/@strid/host-create-react-app-on-azure-986bc40d5bf2#.pycfnafbg) сообщение в блоге или [это](https://github.com/ulrikaugustsson/azure-appservice-static) репозиторий, чтобы узнать, как использовать автоматическое развертывание в службе приложений Azure.

### [Firebase](https://firebase.google.com/)

Установите Firebase CLI, если вы еще этого не сделали, запустив "npm install -g firebase-tools". Зарегистрируйте [учетную запись Firebase](https://console.firebase.google.com/) и создайте новый проект. Запустите `firebase login" и войдите в свою предыдущую учетную запись Firebase.

Затем запустите команду "firebase init" из корневого каталога вашего проекта. Вам нужно выбрать **Хостинг: Настроить и развернуть сайты Firebase Hosting** и выбрать проект Firebase, который вы создали на предыдущем шаге. Вам нужно будет согласиться с созданием "database.rules.json", выбрать "build" в качестве общедоступного каталога, а также согласиться с "Configure в качестве одностраничного приложения", ответив "y`.

```sh
=== Настройка проекта

    Сначала давайте свяжем этот каталог проекта с проектом Firebase.
    Вы можете создать несколько псевдонимов проекта, выполнив команду firebase use --add, но сейчас мы просто настроим проект по умолчанию.

    ? Какой проект Firebase вы хотите связать по умолчанию? Пример приложения (example-app-fd690)

    === Настройка базы данных

    Правила базы данных Firebase в режиме реального времени позволяют вам определить, как должны быть структурированы ваши данные и когда их можно считывать и записывать.

    ? Какой файл следует использовать для правил базы данных? база данных.правила.json
    ✔ Правила базы данных, например, app-fd690, были загружены в database.rules.json.
    Будущие изменения в database.rules.json обновит правила базы данных при запуске
    firebase deploy.

    === Настройка хостинга

    Ваш общий каталог - это папка (относительно каталога вашего проекта), которая будет содержать ресурсы хостинга для загрузки с помощью firebase deploy. Если ты
    если у вас есть процесс сборки для ваших ресурсов, используйте выходной каталог вашей сборки.

    ? Что вы хотите использовать в качестве общедоступного каталога? строить
    ? Настроить как одностраничное приложение (переписать все URL-адреса на /index.html)? Да
    ✔ Написал build/index.html

    я записываю информацию о конфигурации в firebase.json...
    я записываю информацию о проекте в .firebaserc...

    ✔ Инициализация Firebase завершена!
```

ВАЖНО: вам необходимо установить правильные заголовки кэширования HTTP для файла `service-worker.js` в файле `firebase.json`, иначе вы не сможете увидеть изменения после первого развертывания ([проблема #2440](https://github.com/facebookincubator/create-react-app/issues/2440)). Это должно быть добавлено внутри ключа "hosting", как показано ниже:

```
{
  "hosting": {
    ...
    "headers": [
      {"source": "/service-worker.js", "headers": [{"key": "Cache-Control", "value": "no-cache"}]}
    ]
    ...
```

Теперь, после того как вы создадите производственную сборку с помощью "npm run build", вы можете развернуть ее, запустив "firebase deploy`.

```sh
  === Развертывание в "example-app-fd690"...

    я развертываю базу данных, размещаю
    ✔ база данных: правила готовы к развертыванию.
    я размещаю: готовлю каталог сборки для загрузки...
    Загрузка: [============================== ] 75%✔ хостинг: папка сборки успешно загружена
    ✔ хостинг: 8 файлов успешно загружены
    я начинаю процесс выпуска (может занять несколько минут)...

    ✔ Развертывание завершено!

    Консоль проекта: https://console.firebase.google.com/project/example-app-fd690/overview
    URL хостинга: https://example-app-fd690.firebaseapp.com
```

Дополнительные сведения см. в разделе [Добавьте Firebase в свой JavaScript-проект](https://firebase.google.com/docs/web/setup).

### [GitHub Pages](https://pages.github.com/)

> Note: this feature is available with `react-scripts@0.2.0` and higher.

#### Step 1: Add `homepage` to `package.json`

**The step below is important!**<br>
**If you skip it, your app will not deploy correctly.**

Open your `package.json` and add a `homepage` field for your project:

```json
  "homepage": "https://myusername.github.io/my-app",
```

or for a GitHub user page:

```json
  "homepage": "https://myusername.github.io",
```

Приложение Create React использует поле "домашняя страница" для определения корневого URL-адреса в созданном HTML-файле.

#### Шаг 2: Установите "gh-pages" и добавьте "deploy" в "scripts" в "package.json".

Теперь всякий раз, когда вы запускаете "npm run build", вы увидите шпаргалку с инструкциями по развертыванию на страницах GitHub.

Чтобы опубликовать ее на [https://myusername.github.io/my-app](https://myusername.github.io/my-app), запустите:

```sh
npm install --save gh-pages
```

Alternatively you may use `yarn`:

```sh
yarn add gh-pages
```

Add the following scripts in your `package.json`:

```diff
  "scripts": {
+   "predeploy": "npm run build",
+   "deploy": "gh-pages -d build",
    "start": "react-scripts start",
    "build": "react-scripts build",
```

Сценарий "предварительного развертывания" запустится автоматически перед запуском "развертывания".

Если вы выполняете развертывание на странице пользователя GitHub, а не на странице проекта, вам потребуется внести два
дополнительных изменения:

1. Сначала измените исходную ветку вашего репозитория на любую другую, кроме **master**.
1. Кроме того, настройте свои скрипты `package.json`, чтобы отправлять развертывания в **master.**:

```diff
  "scripts": {
    "predeploy": "npm run build",
-   "deploy": "gh-pages -d build",
+   "deploy": "gh-pages -b master -d build",
```

#### Шаг 3: Разверните сайт, выполнив команду `npm run deploy`.

Then run:

```sh
npm run deploy
```

#### Шаг 4: Убедитесь, что в настройках вашего проекта используется `gh-pages`

Наконец, убедитесь, что параметр "Страницы GitHub" в настройках вашего проекта GitHub настроен на использование ветки `gh-pages`:

<img src="http://i.imgur.com/HUjEr9l.png" width="500" alt="настройка ветки gh-pages">

#### Шаг 5: При необходимости настройте домен.

Вы можете настроить пользовательский домен с помощью GitHub Pages, добавив файл "CNAME" в папку "public/".

#### Заметки о маршрутизации на стороне клиента

GitHub Pages не поддерживает маршрутизаторы, которые используют HTML5 "pushState" history API (например, React Router использует "browserHistory`). Это связано с тем, что при загрузке новой страницы по URL-адресу, подобному "http://user.github.io/todomvc/todos/42", где "/todos/42" является интерфейсным маршрутом, сервер страниц GitHub возвращает значение 404, потому что ему ничего не известно о `/todos/42`. Если вы хотите добавить маршрутизатор в проект, размещенный на страницах GitHub, вот несколько решений:

- Вы могли бы переключиться с использования HTML5 history API на маршрутизацию с использованием хэшей. Если вы используете React Router, вы можете переключиться на "hashHistory" для достижения этого эффекта, но URL-адрес будет длиннее и более подробный (например, `http://user.github.io/todomvc/#/todos/42?_k=yknaj`). [Подробнее](https://reacttraining.com/react-router/web/api/Router) о различных реализациях истории в React Router.
- В качестве альтернативы, вы можете использовать трюк, чтобы научить страницы GitHub обрабатывать 404, перенаправив их на вашу страницу "index.html`со специальным параметром перенаправления. Перед развертыванием вашего проекта вам потребуется добавить файл "404.html" с кодом перенаправления в папку "build", а также добавить код, обрабатывающий параметр перенаправления, в`index.html`. Вы можете найти подробное объяснение этого метода [в этом руководстве](https://github.com/rafrex/spa-github-pages).

#### Устранение неполадок

##### "/dev/tty: нет такого устройства или адреса"

Если при развертывании вы получаете сообщение "/dev/tty: нет такого устройства или адреса" или аналогичную ошибку, попробуйте выполнить следующее:

1. Create a new [Personal Access Token](https://github.com/settings/tokens)
2. `git remote set-url origin https://<user>:<token>@github.com/<user>/<repo>` .
3. Try `npm run deploy again`

### [Heroku](https://www.heroku.com/)

Use the [Heroku Buildpack for Create React App](https://github.com/mars/create-react-app-buildpack).<br>
You can find instructions in [Deploying React with Zero Configuration](https://blog.heroku.com/deploying-react-with-zero-configuration).

#### Устранение ошибок при развертывании Heroku

Иногда "npm run build" работает локально, но при развертывании через Heroku происходит сбой. Ниже приведены наиболее распространенные причины.

##### "Модуль не найден: Ошибка: Не удается разрешить "файл" или "каталог""

Если вы получаете что-то вроде этого:

```
remote: Failed to create a production build. Reason:
remote: Module not found: Error: Cannot resolve 'file' or 'directory'
MyDirectory in /tmp/build_1234/src
```

Это означает, что вам нужно убедиться, что регистр букв в файле или каталоге, который вы "импортируете", совпадает с тем, который вы видите в своей файловой системе или на GitHub.

Это важно, потому что Linux (операционная система, используемая Heroku) чувствительна к регистру. Таким образом, "MyDirectory" и "mydirectory" - это два разных каталога, и, таким образом, несмотря на то, что проект создается локально, разница в регистре нарушает инструкции "import" в Heroku remotes.

##### "Не удалось найти требуемый файл".

Если вы исключите или проигнорируете необходимые файлы из пакета, вы увидите ошибку, аналогичную этой:

```
remote: Could not find a required file.
remote:   Name: `index.html`
remote:   Searched in: /tmp/build_a2875fc163b209225122d68916f1d4df/public
remote:
remote: npm ERR! Linux 3.13.0-105-generic
remote: npm ERR! argv "/tmp/build_a2875fc163b209225122d68916f1d4df/.heroku/node/bin/node" "/tmp/build_a2875fc163b209225122d68916f1d4df/.heroku/node/bin/npm" "run" "build"
```

In this case, ensure that the file is there with the proper lettercase and that’s not ignored on your local `.gitignore` or `~/.gitignore_global`.

### [Netlify](https://www.netlify.com/)

**Выполнить ручное развертывание в CDN Netlify:**

```sh
npm install netlify-cli -g
netlify deploy
```

Выберите `build` в качестве пути для развертывания.

\***\*Чтобы настроить непрерывную доставку:**

С помощью этой настройки Netlify будет выполнять сборку и развертывание при нажатии на git или открытии запроса на извлечение:

1. [Запустите новый проект netlify](https://app.netlify.com/signup)
2. Выберите свой Git-хостинг и репозиторий
3. Установите `yarn build` в качестве команды сборки и `build` в качестве каталога публикации
4. Нажмите `Развернуть сайт`

**Поддержка маршрутизации на стороне клиента:**

Для поддержки "pushState" обязательно создайте файл "public/\_redirects" со следующими правилами перезаписи:

```
/*  /index.html  200
```

Когда вы создадите проект, приложение Create React App поместит содержимое папки `public` в выходные данные сборки.

### [Сейчас](https://zeit.co/now)

Теперь предлагается развертывание с нулевой конфигурацией с помощью одной команды. Вы можете использовать `now` для бесплатного развертывания своего приложения.

1. Установите инструмент командной строки `now` либо с помощью рекомендуемого [desktop tool](https://zeit.co/download), либо с помощью node с помощью `npm install -g now`.

2. Создайте свое приложение, запустив `npm run build`.

3. Перейдите в каталог сборки, запустив `cd build`.

4. Запустите `now -name your-project-name` из каталога сборки. В выходных данных вы увидите URL-адрес **now.sh**, который выглядит следующим образом:

   ```
   > Готово! https://your-project-name-tpspyhtdtk.now.sh (скопировано в буфер обмена)
   ```

   Вставьте этот URL-адрес в свой браузер, когда сборка будет завершена, и вы увидите свое развернутое приложение.

Подробности доступны в [этой статье.](https://zeit.co/blog/unlimited-static)

### [S3](https://aws.amazon.com/s3) и [CloudFront](https://aws.amazon.com/cloudfront/)

Смотрите это [сообщение в блоге](https://medium.com/@omgwtfmarc/deploying-create-react-app-to-s3-or-cloudfront-48dae4ce0af) о том, как развернуть ваше приложение React в Amazon Web Services S3 и CloudFront.

### [Surge](https://surge.sh/)

Установите интерфейс командной строки Surge, если вы еще этого не сделали, запустив "npm install -g surge". Выполните команду "surge" и войдите в систему или создайте новую учетную запись.

Когда вас спросят о пути к проекту, обязательно укажите папку "сборка", например:

```sh
       project path: /path/to/project/build
```

Обратите внимание, что для поддержки маршрутизаторов, использующих HTML5 "pushState" API, вы можете переименовать `index.html` в вашей папке сборки в `200.html` перед развертыванием в Surge. Это [гарантирует, что все URL-адреса будут возвращаться к этому файлу](https://surge.sh/help/adding-a-200-page-for-client-side-routing).

## Расширенная настройка

Вы можете настроить различные параметры разработки и производства, установив переменные среды в своей командной строке или с помощью [.env](#добавление переменных среды разработки в env).

| Variable            |      Development       |     Production     | Usage                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| :------------------ | :--------------------: | :----------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BROWSER             |   :white_check_mark:   |        :x:         | By default, Create React App will open the default system browser, favoring Chrome on macOS. Specify a [browser](https://github.com/sindresorhus/opn#app) to override this behavior, or set it to `none` to disable it completely. If you need to customize the way the browser is launched, you can specify a node script instead. Any arguments passed to `npm start` will also be passed to this script, and the url where your app is served will be the last argument. Your script's file name must have the `.js` extension.                                                                                                                                                |
| HOST                |   :white_check_mark:   |        :x:         | By default, the development web server binds to `localhost`. You may use this variable to specify a different host.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| PORT                |   :white_check_mark:   |        :x:         | By default, the development web server will attempt to listen on port 3000 or prompt you to attempt the next available port. You may use this variable to specify a different port.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| HTTPS               |   :white_check_mark:   |        :x:         | When set to `true`, Create React App will run the development server in `https` mode.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| PUBLIC_URL          |          :x:           | :white_check_mark: | Create React App assumes your application is hosted at the serving web server's root or a subpath as specified in [`package.json` (`homepage`)](#building-for-relative-paths). Normally, Create React App ignores the hostname. You may use this variable to force assets to be referenced verbatim to the url you provide (hostname included). This may be particularly useful when using a CDN to host your application.                                                                                                                                                                                                                                                        |
| CI                  | :large_orange_diamond: | :white_check_mark: | When set to `true`, Create React App treats warnings as failures in the build. It also makes the test runner non-watching. Most CIs set this flag by default.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| REACT_EDITOR        |   :white_check_mark:   |        :x:         | When an app crashes in development, you will see an error overlay with clickable stack trace. When you click on it, Create React App will try to determine the editor you are using based on currently running processes, and open the relevant source file. You can [send a pull request to detect your editor of choice](https://github.com/facebookincubator/create-react-app/issues/2636). Setting this environment variable overrides the automatic detection. If you do it, make sure your systems [PATH](<https://en.wikipedia.org/wiki/PATH_(variable)>) environment variable points to your editor’s bin folder. You can also set it to `none` to disable it completely. |
| CHOKIDAR_USEPOLLING |   :white_check_mark:   |        :x:         | When set to `true`, the watcher runs in polling mode, as necessary inside a VM. Use this option if `npm start` isn't detecting changes.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| GENERATE_SOURCEMAP  |          :x:           | :white_check_mark: | When set to `false`, source maps are not generated for a production build. This solves OOM issues on some smaller machines.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| NODE_PATH           |   :white_check_mark:   | :white_check_mark: | Same as [`NODE_PATH` in Node.js](https://nodejs.org/api/modules.html#modules_loading_from_the_global_folders), but only relative folders are allowed. Can be handy for emulating a monorepo setup by setting `NODE_PATH=src`.                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

## Устранение неполадок

### `npm start` не обнаруживает изменений

При сохранении файла во время работы "npm start" браузер должен обновиться с обновленным кодом.
Если этого не произойдет, попробуйте одно из следующих решений.:

- Если ваш проект находится в папке Dropbox, попробуйте переместить его оттуда.
- Если программа просмотра не видит файл с именем "index.js", а вы ссылаетесь на него по имени папки, вам [необходимо перезапустить программу просмотра](https://github.com/facebookincubator/create-react-app/issues/1164) из-за ошибки Webpack.
- В некоторых редакторах, таких как Vim и IntelliJ, есть функция “безопасной записи”, которая в настоящее время нарушает работу наблюдателя. Вам нужно будет отключить ее. Следуйте инструкциям в разделе [“Настройка текстового редактора”](https://webpack.js.org/guides/development/#adjusting-your-text-editor).
- Если путь к вашему проекту содержит круглые скобки, попробуйте переместить проект в путь без них. Это вызвано [ошибкой Webpack watcher](https://github.com/webpack/watchpack/issues/42).
- В Linux и macOS вам может потребоваться [изменить системные настройки](https://github.com/webpack/docs/wiki/troubleshooting#not-enough-watchers), чтобы включить больше наблюдателей.
- Если проект выполняется на виртуальной машине, такой как (Vagrant provisioned) VirtualBox, создайте файл `.env` в каталоге вашего проекта, если он не существует, и добавьте к нему `CHOKIDAR_USEPOLLING=true`. Это гарантирует, что при следующем запуске "npm start" наблюдатель будет использовать режим опроса, если это необходимо внутри виртуальной машины.

Если ни одно из этих решений не поможет, пожалуйста, оставьте комментарий [в этой теме](https://github.com/facebookincubator/create-react-app/issues/659).

### "npm-тест` зависает в macOS Sierra

Если вы запустите "npm test" и консоль зависнет после вывода "react-scripts test --env=jsdom" на консоль, возможно, возникла проблема с вашей установкой [Watchman](https://facebook.github.io/watchman/), как описано в [facebookincubator/create-react-app#713](https://github.com/facebookincubator/create-react-app/issues/713).

Мы рекомендуем сначала удалить "node_modules" в вашем проекте и запустить "npm install" (или "yarn", если вы его используете). Если это не поможет, вы можете попробовать одно из многочисленных обходных решений, упомянутых в этих вопросах:

- [facebook/шутка#1767](https://github.com/facebook/jest/issues/1767)
- [facebook/сторож#358](https://github.com/facebook/watchman/issues/358)
- [ember-cli/эмбер-кли#6259](https://github.com/ember-cli/ember-cli/issues/6259)

Сообщается, что установка Watchman версии 4.7.0 или новее устраняет проблему. Если вы используете [Homebrew](http://brew.sh/), вы можете запустить эти команды, чтобы обновить его.:

```
выключение watchman-
обновление сервера
brew, переустановка watchman
```

Вы можете найти [другие способы установки](https://facebook.github.io/watchman/docs/install.html#build-install) на странице документации Watchman.

Если это по-прежнему не помогает, попробуйте запустить "launchctl unload -F ~/Library/LaunchAgents/com.github.facebook.watchman.plist`.

Также есть сообщения о том, что _uninstalling_ Watchman устраняет проблему. Поэтому, если больше ничего не поможет, удалите его из своей системы и повторите попытку.

### `npm run build` завершается слишком рано

Сообщается, что "npm run build" может завершиться ошибкой на компьютерах с ограниченной памятью и отсутствием пространства подкачки, что часто встречается в облачных средах. Даже в небольших проектах эта команда может увеличить использование оперативной памяти в вашей системе на сотни мегабайт, поэтому, если у вас меньше 1 ГБ доступной памяти, ваша сборка, скорее всего, завершится ошибкой со следующим сообщением:

> Ошибка сборки произошла из-за слишком раннего завершения процесса. Вероятно, это означает, что в системе закончилась память или кто-то вызвал "kill -9" в процессе.

Если вы полностью уверены, что не завершили процесс, подумайте о том, чтобы [добавить немного места для подкачки] (https://www.digitalocean.com/community/tutorials/how-to-add-swap-on-ubuntu-14-04) на компьютере, на котором вы создаете, или создайте проект локально.

### В Heroku не удается выполнить сборку с помощью npm

Возможно, проблема в именах файлов, чувствительных к регистру.
Пожалуйста, ознакомьтесь с [этим разделом] (#устранение ошибок при развертывании heroku).

### Moment.js отсутствуют языковые настройки

Если вы используете [Moment.js](https://momentjs.com/), вы можете заметить, что по умолчанию доступна только английская локаль. Это связано с тем, что файлы языковых стандартов имеют большой размер, и вам, вероятно, понадобится только подмножество [всех языковых стандартов, предоставленных Moment.js](https://momentjs.com/#multiple-locale-support).

Чтобы добавить определенный языковой стандарт Moment.js в свой пакет, вам необходимо импортировать его в явном виде.<br>
Например:

```js
import moment from 'moment'
import 'moment/locale/fr'
```

Если импортировать таким образом несколько языковых стандартов, позже вы сможете переключаться между ними, вызвав `moment.locale()` с именем языкового стандарта:

```js
import moment from 'moment'
import 'moment/locale/fr'
import 'moment/locale/es'

// ...

moment.locale('fr')
```

Это будет работать только для локалей, которые были явно импортированы ранее.

### `npm run build` не удается минимизировать

Некоторые сторонние пакеты не компилируют свой код в ES5 перед публикацией в npm. Это часто вызывает проблемы в экосистеме, поскольку ни браузеры (за исключением большинства современных версий), ни некоторые инструменты в настоящее время не поддерживают все функции ES6. Мы рекомендуем публиковать код на npm как ES5, по крайней мере, еще несколько лет.

<br>
Чтобы решить эту проблему:

1. Откройте проблему в системе отслеживания проблем зависимостей и попросите опубликовать предварительно скомпилированный пакет.

- Примечание: Приложение Create React может использовать как модули CommonJS, так и ES. Для Node.js для обеспечения совместимости рекомендуется, чтобы основной точкой входа был CommonJS. Однако они могут дополнительно предоставить точку входа в модуль ES с полем "module" в "package.json`. Обратите внимание, что ** даже если библиотека предоставляет версию модулей ES, она все равно должна предварительно скомпилировать другие функции ES6 в ES5, если она намерена поддерживать более старые браузеры **.

2. Разветвите пакет и опубликуйте исправленную версию самостоятельно.

3. Если зависимость достаточно мала, скопируйте ее в свою папку "src/" и обрабатывайте как код приложения.

В будущем мы могли бы начать автоматическую компиляцию несовместимых модулей сторонних производителей, но в настоящее время это не поддерживается. Такой подход также замедлит выполнение производственных сборок.

## Альтернативы удалению

[Извлечение](#npm-run-eject) позволяет настраивать все, что угодно, но с этого момента вам придется поддерживать конфигурацию и сценарии самостоятельно. Это может оказаться сложной задачей, если у вас много похожих проектов. В таких случаях вместо удаления мы рекомендуем использовать "react-scripts" и любые другие необходимые вам пакеты. [В этой статье] (https://auth0.com/blog/how-to-configure-create-react-app/) подробно рассказывается о том, как это сделать. Вы можете найти более подробное обсуждение в [этом выпуске](https://github.com/facebookincubator/create-react-app/issues/682).

## Чего-то не хватает?

Если у вас есть идеи о других рецептах, которые должны быть представлены на этой странице, [дайте нам знать](https://github.com/facebookincubator/create-react-app/issues) или [поделитесь своим мнением some!](https://github.com/facebookincubator/create-react-app/edit/master/packages/react-scripts/template/README.md)
