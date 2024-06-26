# Правила ведення репозиторію і стилізації коду

### Правила ведення репозиторію
* Не комітити в гілку main: Всі зміни повинні бути внесені через гілки. В main
повинен бути працючий код, замість прямих комітів у main зливайте
(merge) в неї гілки
* Робити багато маленьких комітів: Це дозволяє зберігати історію роботи і
розуміння змін набагато краще
* Використовувати зрозумілі назви гілок і комітів: Це для розуміння того,
нащо ця гілка була створена або які зміни були внесені в цьому коміті

### Правила стилізації коду
* Назви змінних та методів
  * З назв змінних, функцій, методів і тд має бути зрозуміло, за що вони
відповідають. Назви по типу: a, x, abc, b, fcgvhbjnkml - не підходять
  * Для змінних використовується lowerCamelCase, наприклад: firstName,
lowestDistance
  * Для функцій, методів і класів - CamelCase, наприклад:
CalculateAmount(), ExtractMaxNumber()

* Форматування:
  * Відступи (таби) повинні бути одного розміру (зазвичай 4 пробіли)
  * Після оголошення функції або методу прийнято залишати пустий
рядок, наприклад:
```c#
int CalcSum() { return 0; }
// тут має бути пустий рядок
int CalcAverage() { return 0; }
```
  * Використання var: Краще використувати var де можливо для зменшення
повторень коду і покращення читабельності: замість, наприклад, ```int total = 30;``` пишіть ```var total = 30;```
  * Організація коду: Розділяйте код на логічні блоки за допомогою пропусків,
це покращує читабельність
```c#
var intList = new List<int>() {1, 2, 6, 7, 9};
var filteredList = new List<int>();
// тут має бути пустий рядок, ми оголошували змінні і потім щось робимо у циклі, це два різні логічні блоки
for (var i = 0; i < intList.Count; i++) {//....
```
