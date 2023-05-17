### Что такое метод в javascript?

Метод — это блок кода, который запускается только при вызове.
Вы можете передавать данные, известные как параметры, в метод.
Методы используются для выполнения определенных действий, и они
также известные как функции.

### String в JavaScript
#####Создать строку в javascript
1. Двойные кавычки <span style="color:red; ">`"Idibek"`</span> 
2. Одиночные кавычки <span style="color:red; ">`'Idibek'`</span> 
3. Обратные кавычки <span style="color:red; ">`${variable}`</span>

### Строковые методы JAVASCRIPT

1. `charAt()` 
2. `concat()`
3. `trim()` 
4. `includes()` 
5. `indexOf()`
6. `replace()`
7. `replaceAll()` 
8. `repeat()` 
9. `slice()`
10. `substring()`
11. `split()`
12. `toString()`
13. `toLowerCase()`
14. `toUpperCase()`
15. `at()`


### Числовые методы JavaScript

1. `round()` 
2. `ceil()`
3. `floor()` 
4. `max()` 
5. `min()`
6. `pow()`
7. `sqrt()` 
8. `abs()` 
9. `random()`
10. `isNaN()`




### Метод charAt()
<p>Метод charAt()возвращает указанный символ аз строки.</p>
<p>Индекс первого символа 0, второго 1,...</p>
<p>Индекс последнего символа равен длине length - 1.</p>

    str.charAt(index)
    str.charAt(str.length - 1)

Например:

    let str="Idibek"
    console.log(str.charAt(0))   // output  "I"
    console.log(str.charAt(str.length-1))   // output  "k"

### Метод concat()
<p>Метод concat() объединяет две или более строк.<br>
Метод concat() не изменяет существующие строки.<br>
Метод concat() возвращает новую строку.</p>

Например:

*Объединяет два строк*

    let txt="My name is"
    let Name="Idibek"
    console.log(txt.concat(' ', Name)); // My name is Idibek

*Объединяет три строк*

    let txt="My name is"
    let name="Idibek"
    let surname = "Rahimov"
    console.log(txt.concat(' ', Name,' ',surname)); // My name is Idibek Rahimov


### Метод replace()

Метод replace() ищет в строке значение или регулярное выражение.
Метод replace() возвращает новую строку с замененными значениями.
Метод replace() не изменяет исходную строку.

Например:

    let txt="Microsoft Word"
    console.log(txt.replace("Word","Power Point")); // Microsoft Power Point

###  Метод replaceAll()

Метод replaceAll() возвращает новую строку, в которой все совпадения шаблона заменены новую текст

Например:

    let txt="Microsoft Word, Microsoft PowerPoint, Microsoft Excel, Microsoft Access"
    console.log(txt.replaceAll("Microsoft","Aplication")); // Aplication Word, Aplication PowerPoint, Aplication Excel, Aplication Access


### Метод split()

Метод split() разбивает строку на массив подстрок. Метод split() возвращает новый
множество. Метод split() не изменяет исходную строку. Если в качестве разделителя используется (" "), строка
делится между словами

Например:

    let txt="My name is Idibek"
    console.log(txt.split()); // [ 'My name is Idibek' ]


    let txt="My name is Idibek"
    console.log(txt.split("")); 
    // 
    ['M', 'y', ' ', 'n', 'a',
    'm', 'e', ' ', 'i', 's',
    ' ', 'I', 'd', 'i', 'b',
    'e', 'k']


    let txt="My name is Idibek"
    console.log(txt.split(" ")); // [ 'My', 'name', 'is', 'Idibek' ]

    let txt="My name is Idibek"
    console.log(txt.split(" ",2)); // [ 'My', 'name' ]


##
### Метод substring(start,end)
Метод substring() извлекает символы между двумя индексами (позициями) из строки и возвращает подстроку.
Метод substring() извлекает символы от начала до конца (эксклюзивно).
Метод substring() не изменяет исходную строку.
Если start больше end, аргументы меняются местами: (2, 1) = (1, 2).
Начальное или конечное значения меньше 0 обрабатываются как 0.

Например:


    let firsName="Go to SoftClub"
    let result = firsName.substring(2)
    console.log(result); //  to SoftClub

    let firsName="Go to SoftClub"
    let result = firsName.substring(-3)
    console.log(result); // Go to SoftClub

    let firsName="Go to SoftClub"
    let result = firsName.substring(firsName.length-4)
    console.log(result); // Club

    let firsName="Go to SoftClub"
    let result = firsName.substring(2,firsName.length-4)
    console.log(result); //  to Soft



### Метод slice(start, end)
Метод slice() возвращает неглубокую копию части массива в новый объект массива.
выбрано от начала до конца (конец не включен), где начало и конец представляют индекс элементов в этом массиве.

Например:

    let firsName="Go to SoftClub"
    let result = firsName.slice(5)
    console.log(result); //   SoftClub

    let firsName="Go to SoftClub"
    let result = firsName.slice(-5)
    console.log(result); // tClub

    let firsName="Go to SoftClub"
    let result = firsName.slice(1,-5)
    console.log(result); // o to Sof

    let firsName="Go to SoftClub"
    let result = firsName.slice(-5,-1)
    console.log(result); //  tClu



### Метод toLowerCase()
Метод toLowerCase() преобразует строку в строчные буквы.
Метод toLowerCase() не изменяет исходную строку.

Например:

    let firsName="My Name Is Idibek"
    let result = firsName.toLowerCase()
    console.log(result); // my name is idibek


### Метод toUpperCase()
Метод toUpperCase() преобразует строку в прописные буквы, используя текущую локаль.
Метод toUpperCase() не изменяет исходную строку.

Например:

    let firsName="My Name Is Idibek"
    let result = firsName.toUpperCase()
    console.log(result); // MY NAME IS IDIBEK




### Метод trim()
Метод trim() удаляет пробелы с обеих сторон строки.
Метод trim() не изменяет исходную строку.

Например:

    let firsName="       My Name Is Idibek     "
    let result = firsName.trim()
    console.log(result); // My Name Is Idibek



### Метод includes()
Метод include() возвращает true, если строка содержит указанную строку.
В противном случае он возвращает ложь.
Метод include() чувствителен к регистру.


Например:

    let firsName="Hello Welcome to SoftClub"
    let result = firsName.includes("Welcome")
    console.log(result); // true

    let firsName="Hello Welcome to SoftClub"
    let result = firsName.includes("Welcome",7)
    console.log(result); // false


### Метод toString()
Метод toString() возвращает строку, представляющую объект.
По умолчанию toString() не принимает параметров.

Например:

    let age = 21
    console.log(typeof(age)); // number
    let str = age.toString()
    console.log(typeof(str)); // string




### Метод indexOf()
Метод indexOf() возвращает позицию первого вхождения значения в строку.
Метод indexOf() возвращает -1, если значение не найдено.
Метод indexOf() чувствителен к регистру.

Например:

    let txt = "Welcome to Tajik National University"
    console.log(txt.indexOf("to")); // 8



### Метод repeat()
Метод repeat() создает новую строку, повторяя заданную строку заданное количество раз и возвращает его.


Например:

    let txt = "Welcome"
    console.log(txt.repeat(2)); // WelcomeWelcome


### Метод at()
Метод at() принимает целочисленное значение и возвращает новую строку.
Этот метод позволяет использовать положительные и отрицательные целые числа. Количество отрицательных целых чисел назад от последнего символа строки.

Например:

    let txt = "Welcome to SoftClub"
    console.log(txt.at(4)); // o

    let txt = "Welcome to SoftClub"
    console.log(txt.at(-5)); // t



##

### Метод Math.floor()

Функция Math.floor() округляет число до следующего наименьшего целого числа.

Например:

    let number = 41.2
    console.log(Math.floor(number)); // 41


### Метод Math.round()

Функция Math.round() возвращает число, округленное до ближайшего целого числа.

Например:

    let number = 41.4
    console.log(Math.round(number)); // 41


    let number = 41.6
    console.log(Math.round(number)); // 42


### Метод Math.ceil()

Метод ceil() округляет десятичное число до следующего наибольшего целого числа и возвращает его.

Например:

    let number = 41.4
    console.log(Math.round(number)); // 42



### Метод Math.max()

Метод max() находит максимальное значение среди указанных значений и возвращает его..

Например:

    let number = Math.max(1,2,5,6,8,4,10,232)
    console.log(number); // 232


### Метод Math.min()

Метод min() находит минимальное значение среди указанных значений и возвращает его.

Например:

    let number = Math.min(-1,2,5,6,8,4,10,232)
    console.log(number); // -1


### Метод Math.pow()

Метод pow() вычисляет степень числа, увеличивая второй аргумент. В степени первого аргумента.

Например:

    console.log(Math.pow(2,5)); // 32



### Метод Math.sqrt()

Метод sqrt() вычисляет квадратный корень указанного числа и возвращает его.

Например:

    console.log(Math.sqrt(9)); // 3



### Метод Math.abs()

The abs() method finds the absolute value of the specified number (without any sign) and returns it

Например:

    console.log(Math.abs(-8)); // 8



### Метод Math.random()

Функция random() возвращает псевдослучайное число с плавающей точкой от 0 (включительно)
и 1 (исключительно).

Например:

    console.log(Math.random()); // 0.3906873494603502
    console.log(Math.random()*10); // 7.332646140573389
    console.log(Math.random()*10); // 4.735916158052498



### Метод isNaN()
Функция isNaN() проверяет, является ли значение NaN (Not-a-Number) или нет.

Например:

    let a= NaN
    console.log(isNaN(a)); // true
    let b=5
    console.log(isNaN(b)); // false

