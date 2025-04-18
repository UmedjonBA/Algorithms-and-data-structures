# Такси

**Ограничение времени:** 2 секунды  
**Ограничение памяти:** 256Mb  
**Ввод:** стандартный ввод или input.txt  
**Вывод:** стандартный вывод или output.txt  

## Условие задачи

Как известно, Сан-Фиерро — город одной улицы, то есть все здания лежат на одной прямой. Вы единственный таксист по имени Карл. Нужно развезти группу из \( n \) юношей и \( m \) девушек из клуба по домам. Более того, клуб расположен ровно в начале улицы, то есть всем ехать в одну и ту же сторону. Таким образом, можно всех быстро развезти.  

В такси помещаются 4 человека. Вы доедете до дома того человека, что живет дальше всех, высаживая остальных пассажиров по дороге. Оплата такси — 1 у.е. за километр. Группа не доверяет вам, поэтому молодые люди решили, что в каждом такси должен поехать хотя бы один юноша (но необязательно, чтобы он ехал в такси до самого конца, то есть он может выйти непоследним).  

Найдите способ для молодых людей разделиться на группы и сесть в такси таким образом, что суммарное время будет минимально.  

### Формат ввода  
Первая строка содержит число \( n \) (\( 1 \leq n \leq 2011 \)) — количество юношей. Следующие \( n \) строк содержат имена юношей и расстояния от ночного клуба до их домов (в километрах).  

Далее следует число \( m \) и \( m \) строк, описывающие девушек в том же формате (\( 0 \leq m \leq 2011 \), \( m \leq 3n \)).  

Имена состоят из букв английского алфавита, первая буква заглавная, остальные маленькие. Каждое имя имеет длину от 1 до 15 символов. Никакие два имени не совпадают. Расстояния — неотрицательные целые числа, не превосходящие \( 10^4 \).  

### Формат вывода  
На первой строке выведите минимально возможное время, которые придется заплатить за такси. На второй строке выведите число \( k \) — количество поездок.  

В следующих \( k \) строках выведите, кто поедет в соответствующей поездке. Изучите формат примера и следуйте ему. Вы можете выводить и такси, и люди в произвольном порядке. Если ответ неоднозначен — можете вывести любой.  

### Пример 1  
**Ввод:**  
```
2
Anton 5
Maxim 10
5
Anna 1
Maria 12
Tanya 10
Elena 8
Marina 6
```
**Вывод:**  
```
18
2
Taxi 1: Anton, Marina and Anna.
Taxi 2: Maxim, Maria, Tanya and Elena.
```  

### Пример 2  
**Ввод:**  
```
1
Romeo 100
1
Juliet 200
```  
**Вывод:**  
```
200
1
Taxi 1: Romeo and Juliet.
```  

### Пример 3  
**Ввод:**  
```
1
Jack 17
0
```  
**Вывод:**  
```
17
1
Taxi 1: Jack.
```  

### Примечания  
В данной задаче время и расстояния отождествляются.  
```