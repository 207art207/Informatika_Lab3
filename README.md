# Навігація по документу
- [Титулка](#титулка)
- [Вправа 1](#вправа-1-розширена-8-бiт-кодова-таблиця-ascii-робота-з-розширеною-кодовою-таблицею-ascii-кодова-таблиця-cp1251)
- [Вправа 2](#вправа-2-таблиця-символiв-unicode)
- [Висновок](#висновок)
- [Контрольнi питання](#контрольнi-питання)

## Титулка
<p align="center"><strong>МІНІСТЕРСТВО ОСВІТИ І НАУКИ УКРАЇНИ
<br>НАЦІОНАЛЬНИЙ ТЕХНІЧНИЙ УНІВЕРСИТЕТ УКРАЇНИ
<br>«КИЇВСЬКИЙ ПОЛІТЕХНІЧНИЙ ІНСТИТУТ
<br> ІМЕНІ ІГОРЯ СІКОРСЬКОГО»
<br><br><br>Навчально-науковий інститут телекомунікаційних систем
<br><br>Кафедра телекомунікацій</strong>
<br><br><br><br><br>Дисципліна: «Інформатика. Частина 1.»
<br><strong>ПРОТОКОЛ ВИКОНАННЯ ЛАБОРАТОРНОЇ РОБОТИ № 3</strong> 
<br>«Лабораторна робота 3. Використання
кодових таблиць для представлення
символiв i знакiв у ПК.»</p align="center">
<br><br><br><p align="right">Виконали студенти групи 
<br>ЦС-31 Бригада № 8:
<br>- Шваліковський Вадим
<br>- Шилан Владислав
<br>- Шумлянський Артем
<br><br>Перевірила: 
<br>асистент кафедри ТК 
<br>Олена ФУРТАТ</p>
<br><br><br><p align="center"><strong>КИЇВ 2023</strong></p align="center">

## Вправа 1: Розширена (8-бiт) кодова таблиця ASCII. Робота з розширеною кодовою таблицею ASCII. Кодова таблиця (cp1251).
**Завдання 1**

![Кодова таблиця Windows CP1251](Кодова%20таблиця%20Windows%20CP1251.png)

**Завдання 2**

[![ASCII (Windows cp1251)_Прізвища](ASCII%20(Windows%20cp1251)_Прізвища.png)](ascii.txt) 
## Вправа 2: Таблиця символiв Unicode
**Завдання 1**

![Charmap](Charmap.png)

**Завдання 2**

[![Unicode_Прізвища](Unicode_Прізвища.png)](unicode.txt) 
## Висновок
Завдяки цій лабораторній роботі ми навчилися користуватися HxD редактором, навчилися працювати з кодовими таблицями ASCII, CP1252 та Unicode й дізналися про різні типи кодових таблиць за бітністю.
![Висновок](Висновок.png)

А також дізналися чому розмір [unicode.txt](unicode.txt) більший ніж [ascii.txt](ascii.txt), тому що кодування Unicode використовує одразу два біти для запису одного символу.
## Контрольнi питання
**1.Призначеня кодових таблиць символiв?**

Кодові таблиці використовуються для того, щоб опрацьовувати текстові дані, які кодуються числами.

**2.Кодова таблиця ASCII?**

Кодова таблиця ASCII - система кодів, у якій числа від 0 до 127 включно поставлені у відповідність літерам, цифрам і символам.

**3.Кодова таблиця CP1251?**

Кодова таблиця CP1251 - кодування символів, що є стандартним 8-бітовим кодуванням для всіх версій Microsoft Windows.

**4.Формати символiв в Unicode.**

У Unicode існує кілька різних форматів представлення символів, а саме:

- UTF-8 (Unicode Transformation Format 8-bit): UTF-8 є засобом збереження Unicode-символів у вигляді байтів.  Використовується зазвичай у веб-розробці та в багатьох операційних системах.   Є динамічним кодуванням, що означає, що розмір символу може змінюватися від 1 до 4 байтів, залежно від коду символу.

- UTF-16 (Unicode Transformation Format 16-bit):  UTF-16 зберігає Unicode-символи у вигляді 16-бітних цілих чисел (два байти). Часто використовується в програмуванні й в операційних системах.

- UTF-32 (Unicode Transformation Format 32-bit):   UTF-32 представляє кожен символ Unicode у вигляді 32-бітного цілого числа (чотири байти).   Це найбільш простий формат, але він вимагає більше місця для зберігання тексту.

**5-6.Що означає порядок байтiв Big-endian? Продемонструвати на прикладi.Що означає порядок байтiв Little-endian? Продемонструвати на прикладi.**

Big-endian і Little-endian - це два різних порядки байтів, які використовуються для зберігання багатобайтових чисел у пам'яті комп'ютера. Вони впливають на те, в якому порядку байти представлені у пам'яті, коли велике число розбивається на окремі байти.

У Big-endian порядок байтів, найбільш значущий байт (старший байт) знаходиться в початку числа, а менш значущі байти (молодші байти) слідують за ним. Це означає, що найважливіші біти числа розташовані у початку пам'яті.

Приклад числа 0x12345678 (це число складається з чотирьох байтів):

У Big-endian порядку байтів воно зберігається так:

0x12 0x34 0x56 0x78

У Little-endian порядку байтів це ж число зберігається так:

0x78 0x56 0x34 0x12

**7.Призначення hex-редактора HxD. Продемонструвати на прикладах кодування символiв у форматi Unicode.**

Призначення hex-редактора HxD: редагування даних, які представлені в «сирому вигляді» - як послідовність байтів.
[![приклад кодування символiв у форматi Unicode](Unicode_Прізвища.png)](unicode.txt)

**8.Призначення програми Windows Таблиця символiв. Продемонструвати основнi функцiї.**

Призначення програми Windows Таблиця символiв: за допомогою цієї програми можна копіювати окремі символи або групи символів до буфера обміну, а потім вставляти їх у програми, які підтримують їх відтворення, а також за допомогою неї можна дізнатися коди цих символів у різних форматах кодування.

![Charmap приклад](Charmap.png)




