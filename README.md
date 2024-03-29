## Телефонная книга

Напишите программу, представляющую телефонную книгу. Программа должна иметь следующие функции:

**add(String name, Integer phoneNum):** Добавляет запись в телефонную книгу.
Если запись с именем name уже существует, добавляет новый номер телефона в существующую запись.
Если запись с именем name не существует, создает новую запись с этим именем и номером телефона phoneNum.

**find(String name):** Поиск номеров телефона по имени в телефонной книге.
Если запись с именем name существует, возвращает список номеров телефона для этой записи.
Если запись с именем name не существует, возвращает пустой список.

**getPhoneBook():** Возвращает всю телефонную книгу в виде HashMap, где ключи - это имена, а значения - списки номеров телефона.

Пример.

На входе:
```java
add("Alice", 123456);   
add("Alice", 789012);   
add("Bob", 789012); 
```
  
На выходе:

Команды:

```java
find("Alice")
getPhoneBook()
find("Me")
```

Результат:

```java
[123456, 789012].
{Bob=[789012], Alice=[123456, 789012]}
[]
```


## Задание

Реализуйте структуру телефонной книги с помощью HashMap.

Программа также должна учитывать, что в во входной структуре будут повторяющиеся имена с разными телефонами, их необходимо считать, как одного человека с разными телефонами. Вывод должен быть отсортирован по убыванию числа телефонов.

