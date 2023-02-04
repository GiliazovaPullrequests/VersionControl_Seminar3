# VersionControl_Seminar3
Репозиторий для пулл-реквестов по Введению в контроль версий в Geekbrains

 https://github.com/exquiteble/VersionControl_Seminar3.git

 ## ***_Начальная работа с системой контроля версий_***

<image src="https://miro.medium.com/proxy/1*9PnPjPI65fGwLiMfluVLrw.jpeg" alt="Иконка git">

___

1. >* git --version команда для проверки версии git

___
2. >* ***git init*** **- инициализируем пустой репозиторий**

___
3. >* ***git status*** **- проверяем текущее состояние файла**

___
4. >* ***git add имя файла*** **- добавляем версионность файлу**

___
5. >* ***git add .*** **- добавляет все файлы в папке**

___
6. >* ***git commit - m "Сообщение"*** **- команда для фиксации изменения файла**

___
7. >* ***git commit -am "Сообщение"*** **- фиксация изменений, не требует git add .**

___
8. >* ***git diff*** **- вывод изменений на текущий момент по отношению к последнему коммиту**

___
9. >* ***git log*** **- вся история коммитов в хрон подярдке**

___
10. >* ***git checkout хэш_коммита*** **- переход между изменениями**

___
11. >* ***git checkout master*** **- возрат к текущему состоянию**

___
**Все [цитаты](https://ru.wikiquote.org/wiki/Заглавная_страница) взяты из Википедии.**

>Бёрнса может убить только Бёрнс.

>Смерть? Что вы знаете о смерти?!

>Ад — это место, где отсутствует разум.

___
# Инструкция для работы с Markdown ![git](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Git-logo.svg/640px-Git-logo.svg.png) 

## **Выделение текста**

>(*) - Чтобы выделить тест курсивом.

*Выделенный текст курсивом*

>(**) - Чтобы сделать текст полужирным.

**Текст полужирным**

>_dd_ - курсив (__)

---

## Списки

* Элемент 7 
* Элемент 2
>* Элемент 3
* Элемент 7

(**Элемент 4**)

---
1. Первый пункт
2. Второй пункт

## Работа с изображениями

![Текст](url | or Teftelka.png) - если есть в папке

## Ссылки
__
## Работа с таблицами

___
## Цитаты
>Цитата
___
## Заключение


___

```**Код программы C#:**

using System;

namespace My3
{
     class Program
     {
          static void Main(string[] args)
          {
               Program p = new Program(); // объявляем переменную типа класса Program,
               // чтобы вызвать методы, которые в классе. Т.е. на прямую вызывать нельзя...

               char[] chr = { 'a', 'l', 'e', 'x', 'a', 'n', 'd', 'e', 'r' };
               char[] chr2 = new char[chr.Length]; // копия переменной chr
               Console.Write("chr: ");
               Console.WriteLine(chr);

               // шифрование числов
               for (int i = 0; i < chr.Length; i++)
               {
                    chr2[i] = p.shifr(chr[i],i); // вызов метода шифрования
               }
               Console.Write("chr-shifr: ");
               Console.WriteLine(chr2);
               for (int i = 0; i < chr.Length; i++)
               {
                    chr2[i] = p.shifr(chr2[i], i); // вызов метода дешифрования
               }
               Console.Write("chr-deshifr: ");
               Console.WriteLine(chr2);
               if (!p.ravenstvo(chr,chr2))
               {
                    p.printError("Shifra! "); // вызов метода ошибки шифра
               }

               Console.ReadKey();
          }

          void printError(string s) // наш метод для вывода сообщения ошибки
          {
               Console.Write("Error! " + s + " Press Key...");
               Console.ReadKey();
          }

          char shifr(char x, int shifr) // наш метод для шифрования\дешифрования
          {
               x = (char)(x ^ shifr);
               return x;
          }

          bool ravenstvo(char[] c1, char[] c2) // наш метод для определения равенства
          {
               if (c1.Length == c2.Length)
               {
                    for (int k = 0; k < c1.Length; k++)
                    {
                         if (c1[k] != c2[k]) return false;
                    }
               }
               return true;
          }
     }
}
