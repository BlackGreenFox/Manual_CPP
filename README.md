
### Матеріали | Сайти йдуть у послідовності
- [Informatics](https://informatics.msk.ru/)
- [ACMP Задачі](https://acmp.ru/index.asp?main=tasks)
- [ACM Задачі](https://acm.timus.ru/)
- [Leetcode Задачі](https://leetcode.com/)
- [Hackerrank Задачі](https://www.hackerrank.com/)
- [Codeforcess Мачмейкинг](https://codeforces.com/)
- [Codechef](https://www.codechef.com/)
- [USACO Олімпіада](https://usaco.guide/)

- [C++ ROADMAP]()


### Тема 0 | Точка Входу  
    
### Тема 1.1 | Змінні та типи даних
Усі типи даних мови C++ можна розділити на основні (базові) і складені. Основні типи визначені для представлення цілих, дійсних, символьних і логічних даних. На основі цих типів вводиться опис складених типів, до яких належать масиви, перелічення, функції, структури, посилання, покажчики, об’єднання і класи.

* int (цілий); 
* char (символьний); 
* bool (логічний); 
* float (дійсний);
* double (дійсний з подвійною точністю); 
* void (порожній, не має значення).

> Типи int, char, bool називають цілими, а типи float та double — дійсними з плаваючою крапкою. Код, що формує компілятор для обробки цілих величин, відрізняється від коду для величин з плаваючою крапкою.
 
Для уточнення внутрішнього подання та діапазону значень стандартних типів мова C++ використовує чотири специфікатори типу: 
* short (короткий);
* long (довгий); 
* signed (знаковий); 
* unsigned (беззнаковий).

| Тип                               | Розмір Байт                                             | Значення                                         |
| -------------------------------------- | -----------------------------------------------------------| ----------------------------------------------------------|
| bool | 1 | true або false (0 / 1) |
| unsigned short int | 2 | від 0 до 65535 |
| short int | 2 | від -32768 до 32767 |
| unsigned long int | 4 | від 0 до 4 294 967 295 |
| long int | 4 | від -2 147 483 648 до 2 147 483 647 |
| int(16) | 2 | від -32 768 до 32 767 |
| int(32) | 4 | від -2 147 483 648 до 2 147 483 647 |
| unsigned int (16) | 2 | від 0 до 65535 |
| unsigned int (32) | 4 | від 0 до 4 294 967 295 |
| char | 1 | від 0 до 256 |
| float | 4 | від 1.2е-38 до 3.4е38 |
| double | 8 | від 2.2е-308 до 1.8е308 |
| long double | 10 | від 3.4е-4932 до 3.4е+4932 |

    
### Тема 1.2 | Оператори та вирази
Оператори бувають трьох типів:
* **Унарні**, які працюють з одним операндом. Наприклад, оператор − (мінус). У виразі −7, оператор − застосовується тільки до одного операнду (7) для генерації нового значення (−7).
* **Бінарні**, які працюють з двома операндами (лівим і правим). Наприклад, оператор +. У виразі 5 + 2, оператор + працює з лівим операндом (5) і правим (2) для генерації нового значення (7).
* **Тернарні**, які працюють з трьома операндами. У мові C++ є тільки один тернарний оператор.

> Зверніть увагу, деякі оператори можуть мати кілька значень. Наприклад, оператор − (мінус) може використовуватися в двох контекстах: як унарний оператор для зміни знаку числа (наприклад, конвертувати 7 в −7 і навпаки), і як бінарний для виконання арифметичної операції віднімання (наприклад, 4 − 3).


### Арифметичні оператори:
| Тип                               | Значення                                         |
| -------------------------------------- | ----------------------------------------------------------|
| + | додає два операнди разом |
| - | віднімає один операнд від іншого |
| * | множить два операнди |
| / | ділить один операнд на інший |
| % | повертає остачу від ділення одного операнду на інший | 
```c++
int a = 5;
int b = 3;

// Оператор "+"
int sum = a + b;  // Додаємо значення змінних "a" і "b" і зберігаємо результат в змінній "sum"

// Оператор "-"
int difference = a - b;  // Віднімаємо значення змінної "b" від "a" і зберігаємо результат в змінній "difference"

// Оператор "*"
int product = a * b;  // Множимо значення змінних "a" і "b" і зберігаємо результат в змінній "product"

// Оператор "/"
double division = static_cast<double>(a) / b;  // Ділимо значення змінної "a" на значення змінної "b" і зберігаємо результат в змінній "division"

// Оператор "%"
int remainder = a % b;  // Знаходимо остачу від ділення значення змінної "a" на значення змінної "b" і зберігаємо результат в змінній "remainder"
```
    
    
 ### Оператори присвоєння:   
| Тип                               | Значення                                         |
| -------------------------------------- | ----------------------------------------------------------|
| = | присвоює значення правого операнду лівому операнду |
| += | додає значення правого операнду до лівого операнду і присвоює результат лівому операнду |
| -= | віднімає значення правого операнду від лівого операнду і присвоює результат лівому операнду |
| *= | множить значення лівого операнду на значення правого операнду і присвоює результат лівому операнду |
| /= | ділить значення лівого операнду на значення правого операнду і присвоює результат лівому операнду | 
```c++
int a = 5;
int b = 3;

// Оператор "="
int result1 = a;  // Присвоюємо значення змінної "a" змінній "result1"

// Оператор "+="
result1 += b;  // Додаємо значення змінної "b" до "result1" і присвоюємо результат змінній "result1"

// Оператор "-="
result1 -= b;  // Віднімаємо значення змінної "b" від "result1" і присвоюємо результат змінній "result1"

// Оператор "*="
result1 *= b;  // Множимо значення змінної "result1" на значення змінної "b" і присвоюємо результат змінній "result1"

// Оператор "/="
result1 /= b;  // Ділимо значення змінної "result1" на значення змінної "b" і присвоюємо результат змінній "result1"
```
    
### Оператори порівняння:   
| Тип                               | Значення                                         |
| -------------------------------------- | ----------------------------------------------------------|
| == | пперевіряє, чи рівні два операнди |
| != | перевіряє, чи не рівні два операнди |
| < | перевіряє, чи перший операнд менше другого |
| > | перевіряє, чи перший операнд більше другого |
| <= | перевіряє, чи перший операнд менше або рівний другому |
| >= | перевіряє, чи перший операнд більше або рівний другому |
```c++
int a = 5;
int b = 3;

// Оператор "=="
bool result1 = (a == b);  // Результат: false, оскільки a не дорівнює b

// Оператор "!="
bool result2 = (a != b);  // Результат: true, оскільки a не дорівнює b

// Оператор "<"
bool result3 = (a < b);  // Результат: false, оскільки a не менше b

 // Оператор ">"
bool result4 = (a > b);  // Результат: true, оскільки a більше b

// Оператор "<="
bool result5 = (a <= b);  // Результат: false, оскільки a не менше або рівне b
   
// Оператор ">="
bool result6 = (a >= b);  // Результат: true, оскільки a більше або рівне b
```  
    
### Логічні оператори:   
| Тип                               | Значення                                         |
| -------------------------------------- | ----------------------------------------------------------|
| && | повертає "true", якщо обидва операнди є "true" |
| \|\| | повертає "true", якщо принаймні один операнд є "true" |
| ! | повертає "true", якщо операнд є "false", і навпаки |
```c++
bool a = true;
bool b = false;

// Логічний оператор "&&" (AND)
bool result1 = a && b;  // Результат: false, оскільки обидва операнди не є true
bool result2 = a && !b; // Результат: true, оскільки a = true і !b = true

// Логічний оператор "||" (OR)
bool result3 = a || b;  // Результат: true, оскільки принаймні один операнд (a) є true
bool result4 = !a || b; // Результат: false, оскільки !a = false і b = false

// Логічний оператор "!" (NOT)
bool result5 = !a; // Результат: false, оскільки a = true, а оператор "!" дає зворотне значення

// Використання логічних операторів в умовних виразах (if-else)
if (a && b) {
    // Цей блок коду не виконається, оскільки обидва операнди не є true
    // ...
}
else if (a || b) {
    // Цей блок коду виконається, оскільки принаймні один операнд (a) є true
    // ...
}
else {
    // Цей блок коду не виконається, оскільки всі умови не виконуються
    // ...
}
```   
    
### Побітові оператори:   
| Тип                               | Значення                                         |
| -------------------------------------- | ----------------------------------------------------------|
| \| | побітове І (AND) двох операндів |
| != | побітове АБО (OR) двох операндів |
| ^ | побітове виключне АБО (XOR) двох операндів |
| << | зсув вліво бітів першого операнду на кількість позицій, вказаних другим операндом |
| >> | зсув вправо бітів першого операнду на кількість позицій, вказаних другим операндом |
| ~ | побітовий зворот (NOT) операнду |
```c++
// Побітовий оператор "&" (AND)
int a = 5;  // 0000 0101 в двійковій системі
int b = 3;  // 0000 0011 в двійковій системі
int result1 = a & b;  // Результат: 0000 0001 в двійковій системі (1 в десятковій системі)

// Побітовий оператор "|" (OR)
int result2 = a | b;  // Результат: 0000 0111 в двійковій системі (7 в десятковій системі)

// Побітовий оператор "^" (XOR)
int result3 = a ^ b;  // Результат: 0000 0110 в двійковій системі (6 в десятковій системі)

// Побітовий оператор "<<" (зсув вліво)
int c = 8;  // 0000 1000 в двійковій системі
int result4 = c << 2;  // Результат: 0010 0000 в двійковій системі (32 в десятковій системі)

// Побітовий оператор ">>" (зсув вправо)
int d = 16;  // 0001 0000 в двійковій системі
int result5 = d >> 3;  // Результат: 0000 0010 в двійковій системі (2 в десятковій системі)

// Побітовий оператор "~" (NOT)
int e = 10;  // 0000 1010 в двійковій системі
int result6 = ~e;  // Результат: 1111 0101 в двійковій системі (-11 в десятковій системі)
```  
    
### Оператори інкремента/декремента:
| Тип                               | Значення                                         |
| -------------------------------------- | ----------------------------------------------------------|
| -- |  декремента значення операнду на 1 |
| ++ |  інкрементує значення операнду на 1 |
```c++
int a = 5;
a++; // Результат: a = 6
a--; // Результат: a = 5  
```   
    
    
### Тернарний оператор
| Тип                               | Значення                                         |
| -------------------------------------- | ----------------------------------------------------------|
| ?: | дозволяє зробити умовний вибір |
```c++
int a = 5;
bool b = (a > 10) ? true : false; // Результат: b = false;
```    
    
### Тема 1.3 | Умовні конструкції (if-else, switch)
Для здійснення розгалуження в програмі використовуються так звані умовні оператори
* Оператор if Оператор if робить розгалуження програми залежно від результату перевірки деякої умови на істинність: 
    if (умова) оператор1;
Оператор if Оператор if робить рПараметр умова може бути будь-яким виразом, але найчастіше вираз містить оператори порівняння. Якщо умова, що перевіряється, має істинне значення (true), виконується оператор1. А якщо ні (false), виконання програми переходить до оператора, що йде за умовним оператором.згалуження програми залежно від результату перевірки деякої умови на істинність: 
```c++
if (умова) оператор1;
```
```c++ 
// Спосіб 1
if (b > 0){
    cout << "True"; // Тіло яке спрацює при виконані умови
}

// Спосіб 2
if (b > 0) 
    cout << "True"; // Спрацює при виконані умови

```
    
* Оператор if-else Синтаксис оператора if із ключовим словом else має такий вигляд: 
```c++
if (умова) оператор1; else оператор2;
```
```c++ 
// Спосіб 1
if (b > 0){
    cout << "True"; // Тіло яке спрацює при виконані умови
}
else{
    cout << "False"; // Тіло яке спрацює при НЕ виконані умови
}

// Спосіб 2
if (b > 0) 
    cout << "True"; // Спрацює при виконані умови
else
    cout << "False"; // Спрацює при НЕ виконані умови
```
    
* Оператор if-else if Синтаксис оператора if із ключовим словом else if має такий вигляд: 
```c++
if (умова) оператор1; else if (умова2) оператор2;
```
```c++ 
// Спосіб 1
if (b > 0){
    cout << "True"; // Тіло яке спрацює при виконані умови
}
else if(b == 0){
    cout << "False"; // Тіло яке спрацює при виконані умови2
}

// Спосіб 2
if (b > 0) 
    cout << "True"; // Спрацює при виконані умови
else if(b == 0)
    cout << "False"; // Спрацює при виконані умови2
```

* Замість операторів if-else можна використовувати умовний оператор "? :". Така конструкція має наступний синтаксис: 
```c++
умова ? вираз1 : вираз2;
```
```c++
int a = 10, b = 20, max;
max = (a > b) ? a : b; // Результат: max = 20 ( true : false )
}
```    

* Оператор switch Ще однієї альтернативою керуючої конструкції if-else може служити оператор розгалуження switch.
Синтаксис оператора switch:
```c++
switch(вираз)
{
    case Константа1 : група операторів; break ;
    case Константа2 : група операторів;  break ;
    default Константа3 : група операторів; 
}
```
```c++
switch (вираз) {
    case значення1:
        // Блок коду, який виконується, якщо вираз має значення1
        // Після виконання цього блоку, виконається нижній блок через відсутність break;
    case значення2:
        // Блок коду, який виконується, якщо вираз має значення2
        break;
    ...
    default:
        // Блок коду, який виконується, якщо вираз не має жодного зазначеного значення
        break;
}
```  
    
### Тема 1.4 | Цикли (for, while, do-while)
У мові програмування C++ є три основних типи циклів: цикл "for", цикл "while" і цикл "do-while". Кожен з них дозволяє виконувати блок коду повторно залежно від заданої умови. Опишу кожен з них детально:

* Цикл "for":
Цикл "for" складається з трьох частин: ініціалізація, умова і ітерація. Умова перевіряється перед кожною ітерацією. Якщо умова є істинною, виконується блок коду, після чого відбувається ітерація. Процес повторюється до тих пір, поки умова стає хибною. Ініціалізація виконується лише один раз на початку циклу.
    
```c++
for (ініціалізація; умова; ітерація) {
    // Блок коду, який виконується у кожній ітерації циклу
}
```
```c++
for (int i = 0; i <= 5; i++) {
    cout << i << " ";    // Результат: 0 1 2 3 4 5
}
```  

* Цикл "while":
Цикл "while" перевіряє умову перед кожною ітерацією. Якщо умова є істинною, виконується блок коду. Цикл продовжується, доки умова залишається істинною.

```c++
while (умова) {
    // Блок коду, який виконується, поки умова є істинною
}
```
                 
```c++
int i = 0;

while (i <= 5) {
    cout << i << " ";
    i++;    // Результат: 0 1 2 3 4 5
}
```  

* Цикл "do-while":
Цикл "do-while" спочатку виконує блок коду, а потім перевіряє умову. Якщо умова є істинною, цикл повторюється. Відмінністю цього циклу від "while" є те, що блок коду виконується принаймні один раз, навіть якщо умова вже хибна.
    
```с++
do {
    // Блок коду, який виконується, поки умова є істинною
} while (умова);
```
                 
```c++
int i = 0;

do {
    cout << i << " ";
    i++;
} while (i <= 5);  // Результат: 0 1 2 3 4 5
```  
    
### Тема 1.5 | Функції та повернення значень
У мові програмування C++ функції є основними засобами організації програм та виконання повторюваних завдань. Функції дозволяють групувати певні дії або операції разом та використовувати їх у різних частинах програми. Опишу структуру функції та повернення значень в C++:   
```c++
тип_повернення назва_функції(параметри) {
    // (Тіло) Блок коду, який виконується при виклику функції
    // Операції та дії, які мають бути виконані
    return значення; // Опціональне повернення значення
}
```           
* тип_повернення - це тип даних, який функція повертає після свого виконання. Якщо функція не повертає значення, то використовується тип void. 
* назва_функції - це унікальне ім'я, яке ідентифікує функцію. 
* параметри - це значення, які можуть бути передані у функцію для виконання певних операцій. Параметри є необов'язковими і можуть бути відсутніми. 
* return значення - це опціональна команда для повернення значення з функції. Вона виконується, якщо функція повертає значення.        
                
Функції в C++ можуть повертати значення за допомогою оператора return. Значення, що повертається, повинно бути того ж типу, що й зазначений у типі повернення функції. Якщо функція виконується без повернення значення (тип повернення - void), оператор return може бути пропущений або використаний без значення.
```c++
int Add(int a, int b) {
    int sum = a + b;
    return sum;  // Результат: це сума a і b
}
```         
Приклад використання нашої функції:
```c++
int result = Add(5, 5) // Результат: result = 10
```                
                
Inline-функції - це функції, які можуть бути вбудовані безпосередньо в місце їх виклику. Коли функція оголошується як inline, компілятор може вирішити скопіювати тіло функції в місце виклику, замість фактичного виклику функції. Це може привести до покращення швидкодії програми шляхом уникнення накладних витрат на виклик функції.    
```c++          
inline тип_повернення назва_функції(параметри) {
    // Тіло функції
}        
```    
                
 <details>

<summary>Ремарка як це виглядає зі строни виконання</summary>
Якщо описати нашу функцію так:

```c++
inline int Add(int a, int b)
{
    int result = a + b;
    return result;
}
```
то замість
```c++
cout << Add(2, 2);
```
ми отримаємо розворот функції в набір операторів:

```c++
int result = a + b;
cout << result;
```

</details>

Рекурсія - це процес, коли функція викликає саму себе. Рекурсивні функції розбивають велику задачу на менші частини того ж типу. Кожне викликання функції робить свій внесок у вирішення задачі, а рекурсивні виклики продовжуються досягнення базового випадку, коли рекурсія припиняється. Приклад рекурсивної функції для обчислення факторіала:
```c++
int факторіал(int n) {
    if (n == 0) {
        return 1; // Базовий випадок: факторіал 0 = 1
    } else {
        return n * факторіал(n - 1); // Рекурсивний виклик
    }
}
```
У цьому прикладі функція факторіал використовує рекурсію для обчислення факторіала числа n. Кожен рекурсивний виклик зменшує значення n на 1, аж досягне базового випадку, коли n стає рівним 0. Рекурсія вимагає добре визначеного базового випадку, щоб уникнути безкінечного виконання.

### Тема 2.1 |Огляд синтаксису C++

<details>

<summary> Підключення: </summary>
Підключення #include базової дерективи <iostream> яка допомогає вводити та виводити нам інформацію

```c++
#include <iostream>     // Стандартна бібліотека
#include "file.cpp"     // Ваш файл
```
    
</details>

<details>
<summary> Пространство імен: </summary>
std в C++ є простір імен (namespace), яке містить стандартну бібліотеку C++, також відому як STL (Standard Template Library). Ця бібліотека надає набір класів та функцій, які спрощують розробку програм на C++ та забезпечують загальні алгоритми, структури даних та багато інших корисних інструментів для роботи з даними.

Простір імен std включає безліч підпросторів імен і класів, таких як std::vector, std::string, std::cout, std::cin і багато інших. Вам потрібно вказувати std:: перед ім'ям об'єкта або функції зі стандартної бібліотеки, щоб компілятор міг правильно визначити, до якого саме елемента бібліотеки ви звертаєтесь.
    
```c++
using namespace std;

std::класс/підпространство

```
    
</details>

<details>

<summary> Точка входу в програму: </summary>
Функція main є точкою входу в програму. Вона має повернути ціле значення (зазвичай 0) і може приймати аргументи командного рядка.

```c++
int main() {
    // Тіло функції main
    return 0;
}
```
    
</details>

<details>

<summary> Оголошення змінних: </summary>
тип_даної назва_змінної;

```c++
int value;
```
    
</details>
    
<details>

<summary> Оператори присвоєння: </summary>
змінна = вираз;
    
```c++
int value = 10;
```
    
</details>

<details>
<summary> Ввод та Вивод: </summary>
   
```c++

// Вивод Інформації
// Ці дві конструкції виведуть однаковий результат
std::cout << " Hello " << std::endl;
std::cout << " Hello /n";

// Ввод інформації
std::cin >> value;
```

</details>


### Тема 3.1 | Вказівники (pointers)
Вказівники вказують на адресу пам'яті, де зберігається об'єкт. Вони дозволяють вам працювати з об'єктами, змінювати їх значення та взаємодіяти з пам'яттю більш детально.
* Оголошення вказівників:
```c++

int x = 10;
int *ptr; // Оголошення вказівника
ptr = &x; // Присвоєння вказівнику адреси x

```
* Доступ до значення через вказівник:
```c++

int y = *ptr; // Зчитування значення, на яке вказує вказівник

```
* Зміна значення через вказівник:
```c++

*ptr = 20;

```
* Арифметика вказівників: 
Ви можете додавати або віднімати цілі числа від вказівників, щоб переміщатися по пам'яті.

### Тема 3.2 | Посилання (references):
Посилання - це альтернативний спосіб створення псевдонімів для існуючих об'єктів. Вони не вказують на адресу пам'яті, а забезпечують зручний спосіб робити операції з об'єктом, як змінювати його значення.
* Оголошення посилань:
```c++

int x = 10;
int &ref = x; // Оголошення посилання на x

```
* Зміна значення через посилання:
```c++

ref = 20; // Зміна значення x через посилання ref

```
* Посилання не може бути перевказівненим на інший об'єкт:
```c++

int y = 30;
ref = y; // x тепер буде дорівнювати 30, але ref не можна перевказати на y

```


**Різниця між вказівниками і посиланнями:**

1. Вказівники можуть бути нульовими (не вказувати на жодний об'єкт), в той час як посилання завжди мають вказувати на існуючий об'єкт.
2. Вказівники можуть бути перевказані на інші об'єкти, тоді як посилання залишаються пов'язаними з одним об'єктом протягом свого життєвого циклу.
3. Робота з посиланнями зазвичай більш безпечна і зручна для деяких операцій, тоді як вказівники надають більше контролю над пам'яттю.

Обирайте між вказівниками і посиланнями в залежності від конкретних завдань і потреб вашої програми.

### Тема 3.3 | Посилання (references):
У мові програмування C++, масиви є основною структурою даних для зберігання і керування групами елементів. Масиви можуть бути статичними або динамічними в залежності від того, як виділяється і керується пам'ять для їхніх елементів.
**Статичні масиви:**
Статичний масив визначається на етапі компіляції, і розмір такого масиву відомий на моменті компіляції. Це означає, що розмір і тип кожного елемента масиву визначається до запуску програми. Ось приклад оголошення і використання статичного масиву:
```c++

int staticArray[5]; // Оголошення статичного масиву цілих чисел розміром 5

staticArray[0] = 1; // Присвоєння значення першому елементу
int x = staticArray[2]; // Зчитування значення третього елементу

```
Статичні масиви мають фіксований розмір, який не можна змінювати під час виконання програми. Їх ефективно використовувати, коли ви заздалегідь знаєте розмір масиву і не плануєте змінювати його під час виконання.
**Динамічні масиви:**
Динамічні масиви створюються в режимі виконання програми (в runtime), і їхній розмір може бути змінений за допомогою відповідних функцій. Для створення динамічного масиву використовується оператор new, а для звільнення пам'яті - оператор delete. Ось приклад створення і використання динамічного масиву:
```c++

int* dynamicArray = new int[5]; // Створення динамічного масиву цілих чисел розміром 5

dynamicArray[0] = 1; // Присвоєння значення першому елементу
int y = dynamicArray[2]; // Зчитування значення третього елементу

delete[] dynamicArray; // Звільнення пам'яті, важливо не забути це зробити

```
Однією з головних переваг динамічних масивів є їхній змінюваний розмір. Ви можете виділити пам'ять для масиву та звільнити її, коли вона вам більше не потрібна. Однак важливо дотримуватися правильної практики і завжди звільняти пам'ять, щоб уникнути витоку пам'яті. Обирайте між статичними і динамічними масивами в залежності від конкретних потреб вашої програми та вимог до змінності розміру даних.

### Тема 3.4 |  Пам'ять
У мові програмування C++ для роботи з динамічними масивами використовуються оператори `new`, `delete`, `malloc`, `realloc`, `free` та `sizeof`. Ось приклади використання цих команд:
1. Створення динамічного масиву за допомогою `new` та зміна розміру за допомогою `delete` і `new`:
```c++

int* dynamicArray = new int[5]; // Створення динамічного масиву розміром 5
delete[] dynamicArray; // Звільнення пам'яті

// Зміна розміру масиву
int newSize = 10;
dynamicArray = new int[newSize]; // Створення нового масиву більшого розміру
delete[] dynamicArray; // Звільнення пам'яті попереднього масиву

```
2. Створення динамічного масиву за допомогою `malloc` та зміна розміру за допомогою `realloc`:
```c++

int* dynamicArray = (int*)malloc(5 * sizeof(int)); // Створення динамічного масиву розміром 5
free(dynamicArray); // Звільнення пам'яті

// Зміна розміру масиву
int newSize = 10;
dynamicArray = (int*)realloc(dynamicArray, newSize * sizeof(int)); // Зміна розміру масиву
free(dynamicArray); // Звільнення пам'яті попереднього масиву

```
У вас повинна бути обов'язкова перевірка на успішність виділення пам'яті за допомогою new, malloc або realloc, оскільки ці операції можуть завершитися неуспішно, якщо пам'яті недостатньо.

3. Визначення розміру об'єкта або типу за допомогою `sizeof`:
```c++

int sizeOfInt = sizeof(int); // Отримання розміру типу int в байтах

```
`sizeof` повертає розмір об'єкта або типу в байтах.

Зверніть увагу, що в C++ рекомендується використовувати оператор `new` і оператор `delete` для роботи з динамічними масивами, оскільки вони пов'язані з системою типізації C++ і виконують конструктори та деструктори для об'єктів у масиві. Оператори `malloc`, `realloc` і `free` - це функції мови C і використовуються, коли необхідно інтегрувати код C у C++.



### Тема 4.1 | Struct (структура)
`struct` визначає тип даних, який може містити як дані, так і функції, але за замовчуванням всі члени структури публічні. Це означає, що всі дані структури доступні безпосередньо і можуть бути змінені ззовні об'єкта структури.
* Приклад визначення структури:
```c++

struct Person {
    std::string name;
    int age;
};

```
* Приклад використання структури:
```c++

Person person1;
person1.name = "John";
person1.age = 30;

std::cout << person1.name << " is " << person1.age << " years old." << std::endl;

```
### Тема 4.2 | Class (клас)
`class` також визначає тип даних, але за замовчуванням всі члени класу приватні, тобто недоступні ззовні класу. Це означає, що для доступу до даних і методів класу потрібно використовувати публічні методи, які називаються методами доступу (getters і setters).
* Приклад визначення класу:
```c++

class Person {
private:
    std::string name;
    int age;

public:
    // Конструктор класу
    Person(std::string n, int a) : name(n), age(a) {}

    // Методи доступу для читання та зміни даних
    std::string getName() const {
        return name;
    }

    int getAge() const {
        return age;
    }

    void setName(std::string n) {
        name = n;
    }

    void setAge(int a) {
        age = a;
    }
};

```
* Приклад використання класу:
```c++

Person person1("John", 30);

std::cout << person1.getName() << " is " << person1.getAge() << " years old." << std::endl;

person1.setName("Alice");
person1.setAge(25);

std::cout << person1.getName() << " is now " << person1.getAge() << " years old." << std::endl;

```
**Основні відмінності між `struct` і `class` в C++:**

- В `struct` за замовчуванням всі члени публічні, в `class` - приватні.
- В `class` зазвичай використовуються методи доступу (getters і setters), щоб керувати доступом до даних.
- `class` дає більше контролю над доступом до даних і дозволяє реалізувати інкапсуляцію.


### Тема 5 | Математична бібліотека | cmath

    
```c++

#include <cmath>           // Потрібно підключити для подального використання 

sqrt(число);               // Квадратний корінь числа
pow(число, степінь);       // Піднесення числа до ступеня
abs(число);                // Число в модулі
ceil(число);               // Округлює число в більшу сторону до найближчого цілого
floor(число);              // Округлює число в меншу сторону до найближчого цілого
round(число);              // Округлює число до найближчого цілого за правилами округлення
sin(число);                // Тригонометричні функції синусу
cos(число);                // Тригонометричні функції косінусу
tan(число);                // Тригонометричні функції тангенсу
log(число);                // Число в логарифмі натуральному

```

Також бібліотека має константні значення
[Офіційна документація](https://learn.microsoft.com/ru-ru/cpp/c-runtime-library/math-constants?view=msvc-170)
```c++
#define _USE_MATH_DEFINES  // Треба підключити до #include <cmath>

M_E                        // Число й (близько 2.71828182845904523536)
M_PI                       // Число π (близько 3.14159265358979323846)
M_LOG2E                    // Число log2(e) (близько 1.44269504088896340736)

```
Локальні функції та лямбда-вирази
Функцію можна визначити всередині іншої функції. У C++ для визначення локальних функцій використовують альтернативний синтаксис – так звані лямбда-вирази, які з'явилися в C++ починаючи зі стандарту мови C++11. Лямбда-вираз (lambda expressions) – це вираз для представлення функцій всередині коду. Термін "лямбда" був узятий з математичної теорії рекурсивних функцій, де літера λ використовувалася для позначення функції. Синтаксис лямбда-виразу в C++ виглядає так:

[список захоплення] (список параметрів) { тіло функції }
У список захоплення можна включити імена локальних змінних або параметрів зовнішньої функції. Список захоплення (capture list) і список параметрів можуть бути порожніми. Нижче наведений приклад найпростішого лямбда-виразу:

[](){ cout << "Hello, world!" << endl; }
У найпростішому випадку лямбда-вираз може бути використано для виклику як звичайна функція:

[](){ cout << "Hello, world!" << endl; }();
cout << [](int a, int b) { return a * b; }(2, 2); // 4
Можна створити змінну, яка може бути використана для виклику:

auto f = [](int a, int b) { return a * b; };
cout << f(2, 2); // 4



