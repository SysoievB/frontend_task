```html
-- Сообщаем браузеру как стоит обрабатывать эту страницу -->
<!DOCTYPE html>
<!-- Оболочка документа, указываем язык содержимого -->
<html lang="ru">
	<!-- Заголовок страницы, контейнер для других важных данных (не отображается) -->
	<head>
		<!-- Заголовок страницы в браузере -->
		<title>Мой первый проект</title>
		<!-- Кодировка страницы -->
		<meta http-equiv="Content-type" content="text/html;charset=UTF-8" />
	</head>
	<!-- Отображаемое тело страницы -->
	<body>
		<h1>Ура! Я фрилансер по жизни!!!</h1>
	</body>
</html>
<!-- Формы -->
<!-- Сообщаем браузеру как стоит обрабатывать эту страницу -->
<!DOCTYPE html>
<!-- Оболочка документа, указываем язык содержимого -->
<html lang="ru">
	<!-- Заголовок страницы, контейнер для других важных данных (не отображается) -->
	<head>
		<!-- Заголовок страницы в браузере -->
		<title>Знакомство с HTML тегами. Часть №3 (Формы)</title>
		<!-- Кодировка страницы -->
		<meta http-equiv="Content-type" content="text/html;charset=UTF-8" />
	</head>
	<!-- Отображаемое тело страницы -->
	<body>
		<form action="#" method="post" enctype="multipart/form-data">
			<div>
				<p>Имя</p>
				<input placeholder="Имя" tabindex="1" name="username" type="text" />
			</div>
			<div>
				<p>Пароль</p>
				<input tabindex="2" name="userpass" type="password" />
			</div>
			<div>
				<p>Телефон</p>
				<input tabindex="3" name="userphone" type="tel" />
			</div>
			<div>
				<p>Пол</p>
				<div>
					<input tabindex="4" checked type="radio" name="gender" value="male" /> Мужской
				</div>
				<div>
					<input tabindex="4" type="radio" name="gender" value="female" /> Женский
				</div>
			</div>
			<div>
				<p>Имущество</p>
				<div>
					<input tabindex="5" checked type="checkbox" name="bike" value="yes" /> Велик
				</div>
				<div>
					<input tabindex="6" type="checkbox" name="car" value="yes" /> Машина
				</div>
				<div>
					<input tabindex="7" disabled type="checkbox" name="house" value="yes" /> Дом
				</div>
			</div>
			<div>
				<p>Дополнительная информация</p>
				<textarea tabindex="8" name="text"></textarea>
			</div>
			<div>
				<p>Прикрепить фото</p>
				<input tabindex="9" type="file" />
			</div>
			<div>
				<p>Любимый цвет</p>
				<select tabindex="10" name="color">
					<option value="red">Красный</option>
					<option value="green">Зеленый</option>
					<option selected value="yellow">Желтый</option>
				</select>
			</div>
			<div>
				<p>Действия</p>
				<button tabindex="11" type="submit">Отправить</button>
				<button tabindex="12" type="reset">Очистить</button>
			</div>
		</form>
	</body>
</html>
```
```
=================================================

Основные теги влияющие на отображение страницы

<!-- Кодировка страницы -->
<meta http-equiv="Content-type" content="text/html;charset=UTF-8">
С появлением HTML5 можно использовать 
<meta charset="UTF-8">
<!-- Настройки адаптивности страницы  -->
Фиксированная ширина
<meta name="viewport" content="width=1170">
Адаптивность
<meta name="viewport" content="width=device-width">

<!-- Отключает принудительную ссылку у номера телефона на iOS -->
<meta name="format-detection" content="telephone=no">

=================================================

SEO

<!-- Краткое описание страницы  -->
<meta name="description" content=" ">
Пишем не более 140 символов.
<!-- Ключевые слова страницы  -->
<meta name="keywords" content=" "> 
Пишем не более 20ти слов. Ключевые фразы разделяем запятой.

<!-- Управление доступом поисковых роботов к странице -->
<meta name="robots" content="">

По умолчанию страница индексируется поисковыми система, то есть этот мета тег дополнительно указывать не нужно. Но если задача стоит запретить либо ограничить индексацию, то существуют следующие значения:

none – запретить индексацию страницы полностью.
noindex – запретить индексацию содержимого страницы.
nofollow – игнорировать ссылки в пределах веб-страницы. 
noimageindex - запретить индексацию присутствующих на странице изображений
noarchive - запретить  вывод в результатах поиска ссылки «Сохраненная копия»
nosnippet - запретить  вывод в поисковой выдаче под названием страницы фрагмента текста, описывающего её содержание.

Значения указываются через запятую. Например:

Запрет индексации страницы полностью будет выглядеть так:
<meta name="robots" content="noindex, nofollow">
или так
<meta name="robots" content="none">

Запрет индексации ссылок и изображений на странице будет выглядеть так:
<meta name="robots" content="noimageindex, nofollow">
при этом текст страницы будет доступен к индексации.

=================================================
Технические
<!-- Автор страницы -->
<meta name="Author" content="Пупкин Василий Петрович"> 
<!-- Авторские права -->
<meta name="Copyright" content="Зимина Татьяна Юрьевна"> 
<!-- Адрес автора -->
<meta name="Address" content="Луна, кратер №97">
<!-- Редирект (перезагрузка) страницы. Задержка в секундах; url=Адрес сайта/страницы -->
<meta http-equiv="refresh" content="S; url=URL">

S= Задержка в секундах
URL= Адрес сайта/страницы

=================================================

Для социальных сетей
 
Facebook
Что бы настроить вид нашей страницы в посте мы пишем следующие мета теги:

<!-- локализация сайта, для русскоязычного сайта ru_RU -->
<meta property="og:locale" content="ru_RU">
<!-- тип контента, по умолчанию используется article -->
<meta property="og:type" content="article">
<!-- заголовок страницы, который будет выводится в записи социальной сети -->
<meta property="og:title" content="META теги">
<!-- описание страницы -->
<meta property="og:description" content="Описание страницы про META теги">
<!-- ссылка на изображение, которое будет публиковаться в записи -->
<meta property="og:image" content="http://fls.guru/meta/img/bg.jpg">
<!-- ссылка на текущую страницу -->
<meta property="og:url" content="http://fls.guru/meta/ ">
<!-- название сайта -->
<meta property="og:site_name" content="Фрилансер по жизни">

Проверить разметку можно в валидаторе от Facebook https://developers.facebook.com/tools/debug/sharing/


Подробнее о протоколе Open Graph можно почитать в официальной документации по ссылке в описании. https://ruogp.me/

Для создания Twitter Cards мета теги будут иметь другой вид:

<!-- Тип карты, по умолчанию используется summary -->
<meta name="twitter:card" content="summary">
<!-- Имя/логин автора -->
<meta name="twitter:site" content="Жека">
<!-- Название страницы -->
<meta name="twitter:title" content="META теги">
<!-- Описание страницы -->
<meta name="twitter:description" content="про META теги">
<!-- Cсылка на изображение -->
<meta name="twitter:image" content="http://fls.guru/meta/img/bg.jpg">

Проверяем результат в валидаторе твиттер 
https://cards-dev.twitter.com/validator

Подробнее о создании Twitter Cards можно почитать в официальной документации по ссылке в описании.
https://developer.twitter.com/en/docs/tweets/optimize-with-cards/guides/getting-started
```
