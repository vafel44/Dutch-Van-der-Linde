#РеляционныеБазыДанных #SQL #БазыДанных #Таблицы #Записи #Поля #Связи
#ХранениеДанных #Данные 
#### Реляционные БД

Это тип баз данных, который организует данные в виде таблиц состоящих из строк и столбцов. Каждая таблица представляет собой отношение, где строки(записи) содержат данные содержит данные, а столбцы или поля определяют атрибуты этих данных.
RBD - использует строгую структуру и обеспечивают целостность данных. 
В RBD используются следующие элементы:
- Поля(атрибуты)
- Записи(строки) 
- Ключи
- Индексы
- Ограничения
- Связи между таблицами
### Таблицы

**Таблица** — это основная структура хранения данных в реляционной базе данных. Она состоит из строк и столбцов:

- **Столбцы (поля)**: Каждый столбец таблицы представляет собой атрибут данных. Например, в таблице "Сотрудники" могут быть столбцы "ID", "Имя", "Фамилия", "Должность", "Отдел" и т.д.
    
- **Строки (записи)**: Каждая строка таблицы представляет собой отдельную запись, содержащую данные для каждого из атрибутов. Например, одна строка может содержать информацию о конкретном сотруднике.

### Связи

Связи между таблицами позволяют организовать данные в более сложные структуры и обеспечивают целостность данных. В реляционных базах данных существуют три основных типа связей:

1. **Один к одному (1:1)**:
    
    - В этой связи каждой записи в одной таблице соответствует ровно одна запись в другой таблице. Например, если у вас есть таблица "Сотрудники" и таблица "Паспорт", то каждый сотрудник может иметь только один паспорт, и каждый паспорт принадлежит только одному сотруднику.
2. **Один ко многим (1:N)**:
    
    - В этой связи одной записи в первой таблице может соответствовать несколько записей во второй таблице. Например, в таблице "Отделы" может быть один отдел, в котором работают несколько сотрудников. В этом случае "Отделы" будет первой таблицей, а "Сотрудники" — второй.
3. **Многие ко многим (M:N)**:
    
    - В этой связи одной записи в первой таблице может соответствовать несколько записей во второй таблице, и наоборот. Например, если у вас есть таблицы "Студенты" и "Курсы", то один студент может записаться на несколько курсов, а один курс может включать нескольких студентов. Для реализации такой связи обычно создается промежуточная таблица (например, "Записи"), которая содержит ссылки на обе таблицы.
### Поле

**Поле** (или атрибут) — это отдельный элемент данных в таблице базы данных. Поле представляет собой характеристику или свойство, которое описывает сущность, хранящуюся в таблице. Каждое поле имеет имя и определенный тип данных (например, текст, число, дата), который определяет, какие значения могут быть в этом поле. Например, в таблице "Сотрудники" поля могут включать "Имя", "Фамилия", "Должность", "Зарплата".

### Запись

**Запись** (или кортеж) — это набор связанных полей, который представляет собой одну единицу информации в таблице базы данных. Запись можно рассматривать как строку в таблице, где каждое поле соответствует определенному атрибуту. Например, запись в таблице "Сотрудники" может содержать значения для полей "Имя", "Фамилия", "Должность" и "Зарплата", представляя информацию о конкретном сотруднике.

### Пример

В таблице "Сотрудники":

- Поля: Имя, Фамилия, Должность, Зарплата
- Запись: (Иван, Иванов, Менеджер, 50000)