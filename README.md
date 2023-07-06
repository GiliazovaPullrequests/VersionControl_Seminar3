# VersionControl_Seminar3
Репозиторий для пулл-реквестов по Введению в контроль версий в Geekbrains

Арифметические операторы
C# поддерживает следующие арифметические операторы:

·      (+) – сложение или конкатенация строк;

·      (-) – вычитание;

·      (/) – деление;

·      (*) – умножение;

·      (%) – модуль (взятие остатка).

Операторы (/), (*), (%) имею более высокий приоритет в сравнении с операторами (+), (-). Если операторы имеют один и тот же приоритет, то они выполняются слева направо.

Важно:

Тип результата зависит от типа операндов: выражение 7 / 2 будет иметь значение 3, не 3.5. Результат выражения 7.0 / 2.0 или 7 / 2.0 будет равен 3.5, причем результат будет типа double, не float. В C# числа, имеющие в своей записи точку (.) всегда преобразуются к double.

Логические операторы
Результатом использования таких операторов будет true или false:

·      (==) – равенство выражений;

·      (!=) – отрицание равенства;

·      (!) – отрицание;

·      (<) – меньше;

·      (<=) – меньше, либо равно;

·      (>) – больше;

·      (>=) – больше, либо равно.

·      (&&) – логическое И;

·      (||) – логическое ИЛИ.

Операторы типа
·      is – проверяет, возможно ли преобразование ссылки на объект к определенному типу или интерфейсу;

·      as – не только проверяет, но и преобразует к определенному типу или интерфейсу;

·      typeof – возвращает тип объекта.

Поразрядные операторы
Поразрядные операторы чаще используются с целыми типами данных, но могут использоваться и с логическим типом:

·      (&) – поразрядное И;

·      (|) – поразрядное ИЛИ;

·      (^) – поразрядное исключающее ИЛИ;

·      (>>) – сдвиг вправо, младшие биты отбрасываются, старшие заполняются нулями;

·      (<<) – сдвиг влево, старшие биты отбрасываются, а младшие заполняются нулями.