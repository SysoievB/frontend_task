
1. Создайте пустой объект userInfo.
2. Добавьте свойство name со значением Вася.
3. Добавьте свойство age со значением 30.
4. Измените значение свойства name на Лена.
5. Удалите свойство name из объекта.

```javascript
let userInfo = {

};
userInfo.name = "Vasia";
userInfo.age = 30;
userInfo.name = "Lena";
delete userInfo.name;
console.log(userInfo);
```

Получить верное значение округления
 
 ```javascript
 let numOne = Math.round(1.005 * 100) / 100;
console.log(numOne); // Выведет 1 что не верно

let sourceNum = 1.005 + Number.EPSILON;
let numFour = Math.round(sourceNum * 100) / 100;
console.log(numFour);
 ```

Получить число 135.58 из строки

 ```javascript
 let value = "135.58px";
let value = "135.58px";
console.log(parseFloat(value));//135.58
 ```

Посттроить верное условное ветвление

 ```javascript
 let value = 58 + "Фрилансер";
if (написать ответ) {
	console.log('Результат выражения NaN');
}
 
let value = 58 + "Фрилансер";
if (isNaN(value)) {
	console.log('Результат выражения NaN');
}
 ```

 Найти максимальное число из 10,58,39,-150,0

 ```javascript
 console.log(Math.max(10,58,39,-150,0));//58
 ```

 Округлить число 58.858 до числа 58

 ```javascript
 console.log(Math.floor(58.858));
 ```

Верна ли запись?

 ```javascript
 let fls = "фрилансер";
let text = `Привет! Я ${fls}`;
// Ожидаем получить Привет! Я фрилансер
console.log(text);
 ```

 Получить символ "н" строки:

 ```javascript
 let text = 'фрилансер';
console.log(text[5]);
 ```

 Верно?
```javascript
let text = 123 + "456";
// Ожидаем 579
console.log(text);//123456
```

Получить строку в верхнем регистре

 ```javascript
 let text = 'фрилансер';
console.log(text.toUpperCase());
 ```

 Получить подстроку "лан" из:
```javascript
let text = 'фрилансер';
console.log(text.slice(3,6));
```
 true или false ?

 ```javascript
 let text = 'фрилансер';
console.log(text.includes('лан', 4));//false
 ```

 Какое число (длинну) мы получим?

 ```javascript
 let arr = ['Ваня', 'Иштван', 'Оля',];
let newArr = arr;
newArr.push('Петя');
console.log(arr.length);//4
 ```

Создайте массив users с элементами "Ваня" и "Иштван".
Добавьте "Оля" в конец.
Замените значение в "Иштван" на "Петя".
Ваш код для поиска значения должен
работать для массивов с любой длиной.
Удалите первый элемент массива и покажите его.
Вставьте "Маша" и "Паша" в начало массива.


 ```javascript
 let array = ["Ваня","Иштван",];
array.push("Оля");
for(var i = 0; i < array.length;i++){
	if(array[i] === "Иштван"){
		array[i] = "Петя";
	}
}
let removed = array.splice(1, 1);
console.log(removed);
array.unshift("Маша","Паша");

console.log(array);
 ```

 Удалить элемент 'Иштван' и возвратить его в переменную

 ```javascript
 let arr = ['Ваня', 'Иштван', 'Оля',];
let removed = arr.splice(1, 1);
console.log(removed);
console.log(arr);
 ```

Сделать из строки массив

 ```javascript
 let str = 'Ваня,Иштван,Оля';
let arr = str.split(",");
console.log(arr);
 ```

 Получить в переменную элемент с атрибутом data-say-hi
 и прочитать значение этого атрибута

 ```javascript
 <div data-say-hi="yes">Привет!</div>
const elemsNine = document.querySelector('[data-say-hi="yes"]').outerHTML;
console.log(elemsNine);
 ```

Получить в переменную элемент с текстом Йончи

 ```javascript
 <ul>
	<li>Корчи</li>
	<li>Йончи</li>
</ul>
const elem = document.querySelectorAll('li');
console.log(elem[1]);
 ```

 Получить в переменную коллекцию элементов с классом like

 ```javascript
 <div class="like"></div>
<div class="subscribe"></div>
<div class="like subscribe"></div>
const elem = document.querySelectorAll('div.like');
console.log(elem);
 ```

Узнать ширину полосы прокрутки

 ```javascript
 console.log(window.innerWidth);//1280
 ```

Заставьте браузер прокрутиться на 100px сверху
спустя секунду после открытия страницы

 ```javascript
 function setScrollBy() {
    window.scrollBy(0, parseInt("100px"));
    const windowScrollTop = window.pageYOffset;
    console.log(windowScrollTop);
    }
let myTimeout = setTimeout(setScrollBy, 1000);
console.log(myTimeout);
 ```

Получите координаты любых трех элементов на странице

 ```javascript
 const block = document.querySelector('.lesson__item');
const paragraph = document.querySelector('.lesson__title');
const text = document.querySelector('.lesson__text');

console.log(block.offsetLeft);
console.log(block.offsetTop);

console.log(paragraph.offsetLeft);
console.log(paragraph.offsetTop);

console.log(text.offsetLeft);
console.log(text.offsetTop);
 ```
