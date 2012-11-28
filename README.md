Dev-Workspace
=============

Организация рабочего пространства php веб-разработчика под Windows 7

Версия документа 1.x (xx.xx.2012)

## Инструментарий веб-разработчика (Windows 7)

### Языки программирования, библиотекти, CMS-системы, документация
* **PHP** - [официальная документация](http://www.php.net/manual/ru/)
* **JavaScript** - [документация от Mozilla](https://developer.mozilla.org/en-US/docs/JavaScript), [JavaScript-Garden на русском](http://shamansir.github.com/JavaScript-Garden/)
	* **[jQuery](http://jquery.com/)** - [неофиц. API-документация](http://jqapi.com/), [официальная API](http://api.jquery.com/)
		* **[jQuery Fundamentals](http://jqfundamentals.com/)** - основы jQuery на англ.
		* **[jQuery Boilerplate](http://jqueryboilerplate.com/)** - базовый шаблон плагина на jQuery
		* **[jQuery Plugin Patterns](https://github.com/addyosmani/jquery-plugin-patterns)** - сборник шаблонов плагинов на jQuery
	* **[MooTools](http://mootools.net/)** - [документация](http://mootools.net/docs/core)
* **HTML5** - [документация от Mozilla](https://developer.mozilla.org/ru/docs/HTML/HTML5)
* **CSS3** - [документация от Mozilla](https://developer.mozilla.org/en-US/docs/CSS)
	* **[CSS Compatibility and Internet Explorer](http://msdn.microsoft.com/en-us/library/cc351024)** - поддержка CSS свойств браузерами IE
	* **[Browser Support](http://www.browsersupport.net/)** - поддержка CSS фич браузерами
* Дополнительно по веб-технологиям:
	* **[Dev.Opera](http://dev.opera.com/web)**
	* **[Mozilla Developer Network](https://developer.mozilla.org/)**
	* **[DocHub](http://dochub.io/)** - документация в одном месте по CSS, HTML, JavaScript, DOM, jQuery, PHP
	* **[Can I Use](http://caniuse.com/)** - поддержка современных веб-технологий (HTML, CSS, SVG) браузерами
	* **[HTML5 Boilerplate](http://html5boilerplate.com/)** - базовый шаблон HTML5/CSS3 веб-проекта
	* **[Twitter Bootstrap](http://twitter.github.com/bootstrap/)** - готовый базовый шаблон от Twitter с компонентами
	* **[JavaScript Patterns](http://shichuan.github.com/javascript-patterns/)** - шаблоны в JS
	* **[JavaScript source inspector](http://jsapi.info/)** (jQuery, MooTools и др.) - можно поизучать код библиотек
* **[Contao CMS](https://contao.org/)** - [офиц. документация разработчика](https://contao.org/en/developers-guide.html), [офиц. документация пользователя](https://contao.org/en/users-guide.html), [API](http://api.contao.org/), [англояз. форум](https://community.contao.org/), [багтрекер](https://github.com/contao/core/issues).

### Веб-разработка
* WAMP сервер: [OpenServer](http://open-server.ru/) (apache, mysql, php, ftp, sendmail, cron) - [Установка и настройка](#Локальный-веб-сервер-wamp)
* IDE: [Sublime Text 2](http://www.sublimetext.com/) (php, html, js, css и др.)
* Работа с MySQL: [HeidiSQL](http://www.heidisql.com/) (уже есть в составе OpenServer)
* Система контроля версий: [Mercurial Hg](http://mercurial.selenic.com/) (основная), [SmartGit](http://www.syntevo.com/smartgit/index.html) (для работы с Git)
* Хранение репозиториев онлайн (багтрекер): [Bitbuket](https://bitbucket.org/) (Mercurial, Git), [GitHub](https://github.com/) (Git)
* Бекап файлов и обмен онлайн: [DropBox](https://www.dropbox.com/)
* Работа с ФТП: [WinSCP](http://winscp.net/)
* Работа с SSH: [PuTTY](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html)
* Веб-браузеры: [Chrome](http://www.google.com/intl/ru/chrome/browser/), [Opera](http://opera.com/), [FireFox](http://www.mozilla.org/ru/firefox/), IE, [Safari](http://support.apple.com/kb/DL1531)
* Тестирование устаревших версий браузеров: 
	* IE - [IETester](http://www.my-debugbar.com/wiki/IETester/HomePage)
	* Opera - [Прежние версии](http://www.opera.com/browser/download/?os=windows&list=all) - устанавливать как portable версии

### Верстка
* Инструменты верстальщика: [FastStone Capture](http://www.faststone.org/FSCaptureDetail.htm) (основной), [See Through Windows](http://www.mobzystems.com/tools/seethroughwindows/)
* Публикация скриншотов: [Gyazo](http://gyazo.com/)
* Сжатие PNG изображений: [pngquant](http://pngquant.org/) и [PNGGauntlet](http://pnggauntlet.com/) (использовать оба)
* Сжатие JS: [UglifyJS](https://github.com/mishoo/UglifyJS) (зависит от [nodejs](http://nodejs.org/))
* Сжатие CSS: [YUI Compressor](https://github.com/yui/yuicompressor/downloads)

### Дополнительно
* Хранение паролей: [KeePass](http://keepass.info/)
* Удаленный доступ: [TeamViewer](http://www.teamviewer.com/)
* Виртуализация ОС: [VirtualBox](https://www.virtualbox.org/)
* Работа с изображениями: [FastStone Image Viewer](http://www.faststone.org/FSViewerDetail.htm)
* Работа с документами: [LibreOffice](http://ru.libreoffice.org/)

## Локальный веб-сервер (WAMP)

[OpenServer](http://open-server.ru/) - удобная платформа с гибкой конфигурацией и, самое главное, постоянно развивающаяся.

### Установка и настройка платформы:

* Желательно установить на отдельный виртуальный диск (можно, к примеру, воспользоваться программой [truecrypt](http://www.truecrypt.org/))
* В настройках:
	* создать профиль;
	* вкладка `Модуль` - выбрать `Apache-2.2.x`, `PHP-5.3.x`, `MYSQL-5.1.x`;
	* вкладка `Домены` - проверить чтобы стояло `автоматическое управление списком`;
	* Сохраняем

### Краткое описание работы с платформой

После запуска `Openserver.exe` в трее появится "красный флажок" (это означает что сервер сейчас не запущен). Для запуска сервера кликаем на иконке и выбираем `Запустить`. Ждем запуска. Иногда бывает, что с первого раза сервер не запускается :) - ничего страшного, запускаем воторой раз. В браузере вводим `http://localhost`. Если открылась страница, то все в порядке, сервер работает как надо.

### Настройка php

* Открываем файл конфигурации php:

	![](http://gyazo.com/4b7f182a1421860f1a989e5d3fc06e36.png?1354091588)

* Смотрим, чтобы как минимум были подключены такие расширения (подключены - это значит что вначале строки убран символ `;`):

		extension=php_mbstring.dll
		extension=php_bz2.dll
		extension=php_curl.dll
		extension=php_gd2.dll
		extension=php_imagick.dll
		extension=php_memcache.dll
		extension=php_mysql.dll
		extension=php_mysqli.dll
		extension=php_pdo_mysql.dll
		extension=php_soap.dll

* Устанавливаем временную зону как:

		date.timezone = "Europe/Kiev"

* Также, иногда может понадобится увеличить время выполнения php скрипта. Для этого ищем параметр `max_execution_time` и указываем новое время в секундах выполнения скрипта, например:

		max_execution_time = 60