># Практическая работа №1: Базовые типы данных, консольный ввод-вывод и приведение типов в C#

## Раздел 1. Базовые условия if и if-else



> ### Программа 1. 


```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program1
{
    internal class Program
    {
        static void Main(string[] args)
        {
          //Пользователь вводит целое число. Проверить, является ли оно положительным.
 Console.WriteLine("Введите целое число: ");

 int userInput1 = Convert.ToInt32(Console.ReadLine());

 if (userInput1 > 0) Console.WriteLine("Число положительное - 100%");
 else Console.WriteLine("Точно не положительное - 100%");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/Task3./blob/main/assets/screens/1.png">
</picture>






> ### Программа 2. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program2
{
    internal class Program
    {
        static void Main(string[] args)
        {
           //Пользователь вводит целое число. Проверить, является ли оно четным.
  Console.WriteLine("Введите целое число: ");


 int userInput2 = Convert.ToInt32(Console.ReadLine());

 if (userInput2 % 2 == 0) Console.WriteLine("Число четное - 100%");
 else Console.WriteLine("Точно не четное - 100%");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 3. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program3
{
    internal class Program
    {
        static void Main(string[] args)
        {
          //Даны два целых числа. Вывести наибольшее из них.
 Console.WriteLine("Введите первое число: ");
 int userInput3 = Convert.ToInt32(Console.ReadLine());

 Console.WriteLine("Введите второе число: ");
 int userInput4 = Convert.ToInt32(Console.ReadLine());

 if (userInput3 > userInput4) Console.WriteLine(userInput3);
 else Console.WriteLine(userInput4);
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 4. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program4
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Даны два числа с плавающей точкой. Вывести наименьшее.
Console.WriteLine("Введите первое число: ");
double userInput5 = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Введите второе число: ");
double userInput6 = Convert.ToDouble(Console.ReadLine());

if (userInput5 < userInput6) Console.WriteLine(userInput5);
else Console.WriteLine(userInput6);

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 5. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program5
{
    internal class Program
    {
        static void Main(string[] args)
        {
  //Проверить, делится ли введенное число нацело на 5.
 Console.WriteLine("Введите число: ");


 int userInput7 = Convert.ToInt32(Console.ReadLine());

 if (userInput7 % 5 == 0) Console.WriteLine("Число делится на 5 нацело - 100%");
 else Console.WriteLine("Число НЕ делится на 5 нацело - 100%");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>
---





> ### Программа 6. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program6
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Проверить, оканчивается ли введенное целое число нулем.
 Console.WriteLine("Введите число: ");


 int userInput8 = Convert.ToInt32(Console.ReadLine());

 if (userInput8 % 10 == 0) Console.WriteLine("Число оканчивается нулем - 100%");
 else Console.WriteLine("Число НЕ оканчивается нулем - 100%");
        }
    }
}
        
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 7. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program7
{
    internal class Program
    {
        static void Main(string[] args)
        {
        //Пользователь вводит температуру воздуха. Если она ниже нуля, вывести: «На улице мороз, наденьте шапку».
 Console.WriteLine("Введите температуру воздуха:");


 double userInput9 = Convert.ToDouble(Console.ReadLine());

 if (userInput9 < 0) Console.WriteLine("На улице мороз, наденьте шапку");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 8. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program8
{
    internal class Program
    {
        static void Main(string[] args)
        {
          //Дано число. Если оно больше 100, уменьшить его на 20, иначе увеличить на 10.
  Console.WriteLine("Введите число:");


  double userInput10 = Convert.ToDouble(Console.ReadLine());

  if (userInput10 > 100)
      userInput10 -= 20;
  else
      userInput10 += 10;

  Console.WriteLine(userInput10);
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 9. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program9
{
    internal class Program
    {
        static void Main(string[] args)
        {
         //Ввести два числа. Если они равны, вывести «Числа равны», иначе вывести их произведение.
 

      Console.WriteLine("Введите первое число: ");
      double userInput11 = Convert.ToDouble(Console.ReadLine());

      Console.WriteLine("Введите второе число: ");
      double userInput12 = Convert.ToDouble(Console.ReadLine());

      if (userInput11 == userInput12)
          Console.WriteLine("Числа равны");
      else
          Console.WriteLine($"Произведение чисел: {userInput11 * userInput12}");    
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 10. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program10
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Пользователь вводит свой возраст. Если возраст от 18 и старше, вывести «Доступ разрешен», иначе «Доступ запрещен».
              

     Console.WriteLine("Введите возраст:");


     double userInput13 = Convert.ToDouble(Console.ReadLine());

     if (userInput13 >= 18) Console.WriteLine("Доступ разрешен");
     else
         Console.WriteLine("Доступ запрещен");

        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 11. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program11
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Ввести число. Если оно трехзначное, вывести «Да», иначе «Нет».


     Console.WriteLine("Введите  целое число: ");

     int userInput14 = Convert.ToInt32(Console.ReadLine());

     if (userInput14 >= 100 && userInput14 <= 999) Console.WriteLine("Да");
     else
         Console.WriteLine("Нет");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>








> ### Программа 12. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program12
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Проверить, делится ли число на 3 без остатка.


     Console.WriteLine("Введите  целое число: ");

     int userInput15 = Convert.ToInt32(Console.ReadLine());

     if (userInput15 % 3 == 0)
         Console.WriteLine("Число делится на 3 без остатка");
     else
         Console.WriteLine("Число НЕ делится на 3 без остатка");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 13. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program13
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Даны координаты точки на числовой прямой X.Определить, лежит ли точка правее нуля.


     Console.WriteLine("Введите координату X: ");
     double userInput16 = Convert.ToDouble(Console.ReadLine());

     if (userInput16 > 0)
         Console.WriteLine("Точка лежит правее нуля");
     else
         Console.WriteLine("Точка НЕ лежит правее нуля");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 14. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program14
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Ввести баланс счета. Если баланс отрицательный, вывести «Задолженность!».


     Console.WriteLine("Введите баланс счета: ");
     double userInput17 = Convert.ToDouble(Console.ReadLine());

     if (userInput17 < 0)
         Console.WriteLine("Задолженность!");
     else
         Console.WriteLine("Задолженности нет");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>







> ### Программа 15. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program15
{
    internal class Program
    {
        static void Main(string[] args)
        {
  //Пользователь вводит пароль (целое число). Если введен 1234, вывести «Вход выполнен», иначе «Неверный пароль».
  

      Console.WriteLine("Введите пароль: ");
      int userInput18 = Convert.ToInt32(Console.ReadLine());

      if (userInput18 == 1234)
          Console.WriteLine("Вход выполнен");
      else
          Console.WriteLine("Неверный пароль");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 16. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program16
{
    internal class Program
    {
        static void Main(string[] args)
        {

  //Проверить, является ли введенное число отрицательным.


      Console.WriteLine("Введите число: ");
      double userInput19 = Convert.ToDouble(Console.ReadLine());

      if (userInput19 < 0)
          Console.WriteLine("Число отрицательное");
      else
          Console.WriteLine("Число не отрицательное");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 17. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program17
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Даны два числа. Вывести разность большего и меньшего числа.
               

    Console.WriteLine("Введите первое число: ");
    double userInput20 = Convert.ToDouble(Console.ReadLine());

    Console.WriteLine("Введите второе число: ");
    double userInput21 = Convert.ToDouble(Console.ReadLine());

    if (userInput20 > userInput21)
        Console.WriteLine($"Разность: {userInput20 - userInput21}");
    else
        Console.WriteLine($"Разность: {userInput21 - userInput20}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 18. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program18
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Ввести сумму покупки. Если сумма превышает 1000 рублей, предоставить скидку 5% и вывести итоговую цену.
         

    Console.WriteLine("Введите сумму покупки: ");
    double userInput22 = Convert.ToDouble(Console.ReadLine());

    if (userInput22 > 1000)
        Console.WriteLine($"Итоговая цена со скидкой 5%: {userInput22 * 0.95}");
    else
        Console.WriteLine($"Итоговая цена: {userInput22}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 19. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program19
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Ввести число. Если оно четное, разделить его на 2, если нечетное — умножить на 3.


    Console.WriteLine("Введите число: ");
    double userInput23 = Convert.ToDouble(Console.ReadLine());

    if (userInput23 % 2 == 0)
        Console.WriteLine($"Результат: {userInput23 / 2}");
    else
        Console.WriteLine($"Результат: {userInput23 * 3}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 20. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program20
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Пользователь вводит скорость движения. Если скорость выше 90 км/ч, вывести сообщение о нарушении.


     Console.WriteLine("Введите скорость (км/ч): ");
     double userInput24 = Convert.ToDouble(Console.ReadLine());

     if (userInput24 > 90)
         Console.WriteLine("Нарушение скоростного режима!");
     else
         Console.WriteLine("Скорость в пределах нормы");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 21. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program21
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Дано целое число. Проверить, равно ли оно нулю.
 

     Console.WriteLine("Введите целое число: ");
     int userInput25 = Convert.ToInt32(Console.ReadLine());

     if (userInput25 == 0)
         Console.WriteLine("Число равно нулю");
     else
         Console.WriteLine("Число НЕ равно нулю");


        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 22. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program22
{
    internal class Program
    {
        static void Main(string[] args)
        {


                //Ввести два вещественных числа. Проверить, равны ли они с точностью до 0.001.
                

                    Console.WriteLine("Введите первое число: ");
                    double userInput26 = Convert.ToDouble(Console.ReadLine());

                    Console.WriteLine("Введите второе число: ");
                    double userInput27 = Convert.ToDouble(Console.ReadLine());

                    if (Math.Abs(userInput26 - userInput27) < 0.001)
                        Console.WriteLine("Числа равны с точностью до 0.001");
                    else
                        Console.WriteLine("Числа НЕ равны с точностью до 0.001");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 23. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program23
{
    internal class Program
    {
        static void Main(string[] args)
        {


                //Проверить, делится ли число A на число B без остатка.
                

                    Console.WriteLine("Введите число A: ");
                    int userInput28 = Convert.ToInt32(Console.ReadLine());

                    Console.WriteLine("Введите число B: ");
                    int userInput29 = Convert.ToInt32(Console.ReadLine());

                    if (userInput29 == 0)
                        Console.WriteLine("На ноль делить нельзя");
                    else if (userInput28 % userInput29 == 0)
                        Console.WriteLine("Делится без остатка");
                    else
                        Console.WriteLine("НЕ делится без остатка");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 24. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program24
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Даны два угла треугольника в градусах. Проверить, существует ли такой треугольник (сумма меньше 180).
              

     Console.WriteLine("Введите первый угол: ");
     double userInput30 = Convert.ToDouble(Console.ReadLine());

     Console.WriteLine("Введите второй угол: ");
     double userInput31 = Convert.ToDouble(Console.ReadLine());

     if (userInput30 + userInput31 < 180)
         Console.WriteLine("Треугольник существует");
     else
         Console.WriteLine("Треугольник НЕ существует");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 25. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program25
{
    internal class Program
    {
        static void Main(string[] args)
        {


//Ввести радиус круга и сторону квадрата. Определить, у какой фигуры площадь больше.


    Console.WriteLine("Введите радиус круга: ");
    double userInput32 = Convert.ToDouble(Console.ReadLine());

    Console.WriteLine("Введите сторону квадрата: ");
    double userInput33 = Convert.ToDouble(Console.ReadLine());

    double circleArea = Math.PI * userInput32 * userInput32;
    double squareArea = userInput33 * userInput33;

    if (circleArea > squareArea)
        Console.WriteLine($"Площадь круга больше: {circleArea}");
    else if (squareArea > circleArea)
        Console.WriteLine($"Площадь квадрата больше: {squareArea}");
    else
        Console.WriteLine("Площади равны");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 26. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program26
{
    internal class Program
    {
        static void Main(string[] args)
        {
  //Ввести два числа. Вывести частное большего на меньшее (предусмотреть проверку деления на 0).
 

      Console.WriteLine("Введите первое число: ");
      double userInput34 = Convert.ToDouble(Console.ReadLine());

      Console.WriteLine("Введите второе число: ");
      double userInput35 = Convert.ToDouble(Console.ReadLine());

      if (userInput34 == 0 || userInput35 == 0)
          Console.WriteLine("Деление на ноль невозможно");
      else if (userInput34 > userInput35)
          Console.WriteLine($"Частное: {userInput34 / userInput35}");
      else
          Console.WriteLine($"Частное: {userInput35 / userInput34}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 27. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program27
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Проверить, является ли последняя цифра числа семеркой.
 

     Console.WriteLine("Введите целое число: ");
     int userInput36 = Convert.ToInt32(Console.ReadLine());

     if (Math.Abs(userInput36) % 10 == 7)
         Console.WriteLine("Последняя цифра — семерка");
     else
         Console.WriteLine("Последняя цифра — НЕ семерка");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 28. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program28
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Дано число. Если оно нечетное и положительное, вывести «Да».


    Console.WriteLine("Введите число: ");
    int userInput37 = Convert.ToInt32(Console.ReadLine());

    if (userInput37 > 0 && userInput37 % 2 != 0)
        Console.WriteLine("Да");
    else
        Console.WriteLine("Нет");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 29. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program29
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Ввести объем свободного места на диске (в ГБ). Если места меньше 5 ГБ, вывести предупреждение.


    Console.WriteLine("Введите объем свободного места (ГБ): ");
    double userInput38 = Convert.ToDouble(Console.ReadLine());

    if (userInput38 < 5)
        Console.WriteLine("Внимание! Мало свободного места на диске");
    else
        Console.WriteLine("Свободного места достаточно");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 30. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program30
{
    internal class Program
    {
        static void Main(string[] args)
        {

                //Пользователь вводит оценку (2, 3, 4, 5). Если оценка 4 или 5, вывести «Молодец», иначе «Нужно подтянуться».
                

                    Console.WriteLine("Введите оценку: ");
                    int userInput39 = Convert.ToInt32(Console.ReadLine());

                    if (userInput39 == 4 || userInput39 == 5)
                        Console.WriteLine("Молодец");
                    else
                        Console.WriteLine("Нужно подтянуться");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 31. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program31
{
    internal class Program
    {
        static void Main(string[] args)
        {


                //Даны два символа. Проверить, совпадают ли они.
                

                    Console.WriteLine("Введите первый символ: ");
                    char userInput40 = Convert.ToChar(Console.ReadLine());

                    Console.WriteLine("Введите второй символ: ");
                    char userInput41 = Convert.ToChar(Console.ReadLine());

                    if (userInput40 == userInput41)
                        Console.WriteLine("Символы совпадают");
                    else
                        Console.WriteLine("Символы НЕ совпадают");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 32. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program32
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Ввести число. Если оно кратно и 2, и 7, вывести «Кратно 14».
               

    Console.WriteLine("Введите число: ");
    int userInput42 = Convert.ToInt32(Console.ReadLine());

    if (userInput42 % 2 == 0 && userInput42 % 7 == 0)
        Console.WriteLine("Кратно 14");
    else
        Console.WriteLine("НЕ кратно 14");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 33. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program33
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Ввести массу груза. Если масса превышает допустимые 3.5 тонны, вывести «Перегруз!».


    Console.WriteLine("Введите массу груза (тонн): ");
    double userInput43 = Convert.ToDouble(Console.ReadLine());

    if (userInput43 > 3.5)
        Console.WriteLine("Перегруз!");
    else
        Console.WriteLine("Масса в пределах нормы");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 34. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program34
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Ввести текущее время (часы от 0 до 23). Если время от 6 до 12, вывести «Доброе утро».


    Console.WriteLine("Введите текущий час (0–23): ");
    int userInput44 = Convert.ToInt32(Console.ReadLine());

    if (userInput44 >= 6 && userInput44 <= 12)
        Console.WriteLine("Доброе утро");
    else
        Console.WriteLine("Не утро");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 35. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program35
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Ввести рост человека в см. Если рост больше 200 см, вывести «Очень высокий».


     Console.WriteLine("Введите рост (см): ");
     double userInput45 = Convert.ToDouble(Console.ReadLine());

     if (userInput45 > 200)
         Console.WriteLine("Очень высокий");
     else
         Console.WriteLine("Рост в пределах нормы");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 36. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program36
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Дано двузначное число. Определить, какая из его цифр больше.
 
     Console.WriteLine("Введите двузначное число: ");
     int userInput46 = Convert.ToInt32(Console.ReadLine());

     int firstDigit = Math.Abs(userInput46) / 10;
     int secondDigit = Math.Abs(userInput46) % 10;

     if (firstDigit > secondDigit)
         Console.WriteLine($"Больше первая цифра: {firstDigit}");
     else if (secondDigit > firstDigit)
         Console.WriteLine($"Больше вторая цифра: {secondDigit}");
     else
         Console.WriteLine("Цифры равны");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 37. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program37
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Ввести стоимость товара. Если товар бесплатный (цена 0), вывести «Акция!».
               

    Console.WriteLine("Введите стоимость товара: ");
    double userInput47 = Convert.ToDouble(Console.ReadLine());

    if (userInput47 == 0)
        Console.WriteLine("Акция!");
    else
        Console.WriteLine("Товар платный");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 38. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program38
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Проверить, содержит ли введенное двузначное число одинаковые цифры.
               

    Console.WriteLine("Введите двузначное число: ");
    int userInput48 = Convert.ToInt32(Console.ReadLine());

    int userInput49 = Math.Abs(userInput48) / 10;
    int userInput50 = Math.Abs(userInput48) % 10;

    if (userInput49 == userInput50)
        Console.WriteLine("Цифры одинаковые");
    else
        Console.WriteLine("Цифры разные");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 39. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program39
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Ввести уровень громкости (0–100). Если громкость превышает 80, вывести «Слишком громко для слуха».
               

    Console.WriteLine("Введите уровень громкости (0–100): ");
    int userInput51 = Convert.ToInt32(Console.ReadLine());

    if (userInput51 > 80)
        Console.WriteLine("Слишком громко для слуха");
    else
        Console.WriteLine("Громкость безопасна");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 40. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program40
{
    internal class Program
    {
        static void Main(string[] args)
        {
  //Даны два числа. Если их сумма четная, вывести сумму, иначе вывести их разность.
             

      Console.WriteLine("Введите первое число: ");
      int userInput52 = Convert.ToInt32(Console.ReadLine());

      Console.WriteLine("Введите второе число: ");
      int userInput53 = Convert.ToInt32(Console.ReadLine());

      if ((userInput52 + userInput53) % 2 == 0)
          Console.WriteLine($"Сумма: {userInput52 + userInput53}");
      else
          Console.WriteLine($"Разность: {userInput52 - userInput53}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 41. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program41
{
    internal class Program
    {
        static void Main(string[] args)
        {
  //Ввести количество страниц в документе. Если страниц больше 100, включить двухстороннюю печать.
          

      Console.WriteLine("Введите количество страниц: ");
      int userInput54 = Convert.ToInt32(Console.ReadLine());

      if (userInput54 > 100)
          Console.WriteLine("Включена двухсторонняя печать");
      else
          Console.WriteLine("Обычная печать");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 42. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program42
{
    internal class Program
    {
        static void Main(string[] args)
        {
  //Проверить, является ли введенное целое число полным квадратом (для проверки использовать Math.Sqrt).


      Console.WriteLine("Введите целое число: ");
      int userInput55 = Convert.ToInt32(Console.ReadLine());

      if (userInput55 < 0)
          Console.WriteLine("Отрицательное число не может быть полным квадратом");
      else if (Math.Sqrt(userInput55) == Math.Floor(Math.Sqrt(userInput55)))
          Console.WriteLine("Число является полным квадратом");
      else
          Console.WriteLine("Число НЕ является полным квадратом");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 43. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program43
{
    internal class Program
    {
        static void Main(string[] args)
        {

  //Ввести атмосферное давление. Если давление ниже 740 мм рт. ст., вывести «Пониженное давление».
         

      Console.WriteLine("Введите атмосферное давление (мм рт. ст.): ");
      double userInput56 = Convert.ToDouble(Console.ReadLine());

      if (userInput56 < 740)
          Console.WriteLine("Пониженное давление");
      else
          Console.WriteLine("Давление в норме");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 44. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program44
{
    internal class Program
    {
        static void Main(string[] args)
        {
   //Ввести количество забитых мячей командами А и Б. Вывести победителя или сообщить о ничьей.


       Console.WriteLine("Введите количество мячей команды А: ");
       int userInput57 = Convert.ToInt32(Console.ReadLine());

       Console.WriteLine("Введите количество мячей команды Б: ");
       int userInput58 = Convert.ToInt32(Console.ReadLine());

       if (userInput57 > userInput58)
           Console.WriteLine("Победила команда А");
       else if (userInput58 > userInput57)
           Console.WriteLine("Победила команда Б");
       else
           Console.WriteLine("Ничья");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 45. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program45
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Дано число. Заменить его на абсолютную величину (модуль) без использования Math.Abs.

     Console.WriteLine("Введите число: ");
     double userInput59 = Convert.ToDouble(Console.ReadLine());

     if (userInput59 < 0)
         userInput59 = -userInput59;

     Console.WriteLine($"Модуль числа: {userInput59}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 46. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program46
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Ввести показатель уровня сахара в крови. Если показатель выше 6.1 ммоль/л, вывести «Выше нормы».
              

    Console.WriteLine("Введите уровень сахара (ммоль/л): ");
    double userInput60 = Convert.ToDouble(Console.ReadLine());

    if (userInput60 > 6.1)
        Console.WriteLine("Выше нормы");
    else
        Console.WriteLine("В пределах нормы");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 47. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program47
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Проверить, хватит ли пользователю средств на счете для оплаты проезда стоимостью 35 рублей.
               

    Console.WriteLine("Введите сумму на счете: ");
    double userInput61 = Convert.ToDouble(Console.ReadLine());

    if (userInput61 >= 35)
        Console.WriteLine("Средств достаточно для оплаты проезда");
    else
        Console.WriteLine("Недостаточно средств для оплаты проезда");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 48. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program48
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Ввести номер текущего этажа. Если этаж выше 10, вывести «Высотный этаж».


    Console.WriteLine("Введите номер этажа: ");
    int userInput62 = Convert.ToInt32(Console.ReadLine());

    if (userInput62 > 10)
        Console.WriteLine("Высотный этаж");
    else
        Console.WriteLine("Обычный этаж");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 49. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program49
{
    internal class Program
    {
        static void Main(string[] args)
        {

                //Ввести два слова. Проверить, одинаковы ли они по длине.
                

                    Console.WriteLine("Введите первое слово: ");
                    string userInput63 = Console.ReadLine();

                    Console.WriteLine("Введите второе слово: ");
                    string userInput64 = Console.ReadLine();

                    if (userInput63.Length == userInput64.Length)
                        Console.WriteLine("Слова одинаковой длины");
                    else
                        Console.WriteLine("Слова разной длины");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 50. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program50
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Пользователь вводит целое число. Вывести строковое сообщение: «Число четное» либо «Число нечетное».
               

    Console.WriteLine("Введите целое число: ");
    int userInput65 = Convert.ToInt32(Console.ReadLine());

    if (userInput65 % 2 == 0)
        Console.WriteLine("Число четное");
    else
        Console.WriteLine("Число нечетное");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>












## Раздел 2. Множественные ветвления else if и диапазоны

 ### Программа 51. 


```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program51
{
    internal class Program
    {
        static void Main(string[] args)
        {
          //Ввести балл за тест (0–100). Вывести оценку по шкале ECTS: A (90-100), B (80-89), C (70-79), D (60-69), F (менее 60).


    Console.WriteLine("Введите балл за тест (0–100): ");
    int userInput66 = Convert.ToInt32(Console.ReadLine());

    if (userInput66 >= 90)
        Console.WriteLine("Оценка: A");
    else if (userInput66 >= 80)
        Console.WriteLine("Оценка: B");
    else if (userInput66 >= 70)
        Console.WriteLine("Оценка: C");
    else if (userInput66 >= 60)
        Console.WriteLine("Оценка: D");
    else
        Console.WriteLine("Оценка: F");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 52. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program52
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //Ввести возраст человека. Определить категорию: ребенок (0-12), подросток (13-17), взрослый (18-64), пожилой (65+).


     Console.WriteLine("Введите возраст: ");
     int userInput67 = Convert.ToInt32(Console.ReadLine());

     if (userInput67 <= 12)
         Console.WriteLine("Ребенок");
     else if (userInput67 <= 17)
         Console.WriteLine("Подросток");
     else if (userInput67 <= 64)
         Console.WriteLine("Взрослый");
     else
         Console.WriteLine("Пожилой");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 53. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program53
{
    internal class Program
    {
        static void Main(string[] args)
        {
         
                //Ввести температуру воды. Вывести ее агрегатное состояние: «Лед» (≤0), «Жидкость» (0<t<100), «Пар» (≥100).
        

                    Console.WriteLine("Введите температуру воды: ");
                    double userInput68 = Convert.ToDouble(Console.ReadLine());

                    if (userInput68 <= 0)
                        Console.WriteLine("Лед");
                    else if (userInput68 < 100)
                        Console.WriteLine("Жидкость");
                    else
                        Console.WriteLine("Пар"); 
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 54. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program54
{
    internal class Program
    {
        static void Main(string[] args)
        {
               //Ввести уровень заряда аккумулятора смартфона (в %). Вывести: «Критический» (<10), «Низкий» (10 - 20), «Нормальный» (21 - 80), «Полный» (81 - 100).
       

           Console.WriteLine("Введите уровень заряда (%): ");
           int userInput69 = Convert.ToInt32(Console.ReadLine());

           if (userInput69 < 10)
               Console.WriteLine("Критический");
           else if (userInput69 <= 20)
               Console.WriteLine("Низкий");
           else if (userInput69 <= 80)
               Console.WriteLine("Нормальный");
           else
               Console.WriteLine("Полный");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 55. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program55
{
    internal class Program
    {
        static void Main(string[] args)
        {
           //Ввести число оборотов двигателя в минуту (RPM). Вывести режим: «Заглушен» (0), «Холостой ход» (1-900), «Рабочий» (901-3500), «Красная зона» (3501+).
 

      Console.WriteLine("Введите число оборотов (RPM): ");
      int userInput70 = Convert.ToInt32(Console.ReadLine());

      if (userInput70 == 0)
          Console.WriteLine("Заглушен");
      else if (userInput70 <= 900)
          Console.WriteLine("Холостой ход");
      else if (userInput70 <= 3500)
          Console.WriteLine("Рабочий");
      else
          Console.WriteLine("Красная зона");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>
---





> ### Программа 56. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program56
{
    internal class Program
    {
        static void Main(string[] args)
        {
   //Ввести сумму дохода за год. Рассчитать подоходный налог: до 2.4 млн — 13%, до 5 млн — 15%, выше 5 млн — 18%.
            

       Console.WriteLine("Введите сумму дохода за год: ");
       double userInput71 = Convert.ToDouble(Console.ReadLine());

       if (userInput71 <= 2400000)
           Console.WriteLine($"Налог: {userInput71 * 0.13}");
       else if (userInput71 <= 5000000)
           Console.WriteLine($"Налог: {userInput71 * 0.15}");
       else
           Console.WriteLine($"Налог: {userInput71 * 0.18}");
        }
    }
}
        
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 57. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program57
{
    internal class Program
    {
        static void Main(string[] args)
        {
         //По введенной координате X точки на плоскости(при Y = 0) определить ее положение: на нуле, в положительной или отрицательной полуоси.


     Console.WriteLine("Введите координату X: ");
     double userInput72 = Convert.ToDouble(Console.ReadLine());

     if (userInput72 == 0)
         Console.WriteLine("Точка на нуле");
     else if (userInput72 > 0)
         Console.WriteLine("Точка в положительной полуоси");
     else
         Console.WriteLine("Точка в отрицательной полуоси");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 58. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program58
{
    internal class Program
    {
        static void Main(string[] args)
        {
              //Ввести индекс массы тела (ИМТ). Вывести категорию: дефицит веса (< 18.5), норма(18.5 - 24.9), избыток(25 - 29.9), ожирение(30 +).
   

         Console.WriteLine("Введите ИМТ: ");
         double userInput73 = Convert.ToDouble(Console.ReadLine());

         if (userInput73 < 18.5)
             Console.WriteLine("Дефицит веса");
         else if (userInput73 < 25)
             Console.WriteLine("Норма");
         else if (userInput73 < 30)
             Console.WriteLine("Избыток");
         else
             Console.WriteLine("Ожирение");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 59. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program59
{
    internal class Program
    {
        static void Main(string[] args)
        {
           
                //Ввести скорость ветра (м/с). Вывести категорию по шкале: штиль (<0.2), легкий ветерок(0.2 - 5), умеренный(5.1 - 14), шторм(14.1 - 24), ураган(>24).
              

                    Console.WriteLine("Введите скорость ветра (м/с): ");
                    double userInput74 = Convert.ToDouble(Console.ReadLine());

                    if (userInput74 < 0.2)
                        Console.WriteLine("Штиль");
                    else if (userInput74 <= 5)
                        Console.WriteLine("Легкий ветерок");
                    else if (userInput74 <= 14)
                        Console.WriteLine("Умеренный");
                    else if (userInput74 <= 24)
                        Console.WriteLine("Шторм");
                    else
                        Console.WriteLine("Ураган");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 60. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program60
{
    internal class Program
    {
        static void Main(string[] args)
        {
      //Ввести стаж работы сотрудника (в годах). Вывести размер надбавки: <1года — 0 %, 1 - 5 лет — 5 %, 6 - 10 лет — 10 %, >10 лет — 15 %.
      

          Console.WriteLine("Введите стаж работы (лет): ");
          double userInput75 = Convert.ToDouble(Console.ReadLine());

          if (userInput75 < 1)
              Console.WriteLine("Надбавка: 0%");
          else if (userInput75 <= 5)
              Console.WriteLine("Надбавка: 5%");
          else if (userInput75 <= 10)
              Console.WriteLine("Надбавка: 10%");
          else
              Console.WriteLine("Надбавка: 15%");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 61. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program61
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Пользователь вводит текущий час (0–23). Вывести: «Ночь» (0-5), «Утро» (6-11), «День» (12-17), «Вечер» (18-23).
 

     Console.WriteLine("Введите текущий час (0–23): ");
     int userInput76 = Convert.ToInt32(Console.ReadLine());

     if (userInput76 <= 5)
         Console.WriteLine("Ночь");
     else if (userInput76 <= 11)
         Console.WriteLine("Утро");
     else if (userInput76 <= 17)
         Console.WriteLine("День");
     else
         Console.WriteLine("Вечер");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>








> ### Программа 62. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program62
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Ввести толщину льда на водоеме (см). Вывести: «Выход запрещен» (<7), «Одиночный пешеход» (7 - 12), «Группа людей» (13 - 20), «Транспорт» (>20).


     Console.WriteLine("Введите толщину льда (см): ");
     double userInput77 = Convert.ToDouble(Console.ReadLine());

     if (userInput77 < 7)
         Console.WriteLine("Выход запрещен");
     else if (userInput77 <= 12)
         Console.WriteLine("Одиночный пешеход");
     else if (userInput77 <= 20)
         Console.WriteLine("Группа людей");
     else
         Console.WriteLine("Транспорт");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 63. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program63
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Даны три целых числа A, B, C. Найти максимальное из них, используя каскадное условие.


    Console.WriteLine("Введите число A: ");
    int userInput78 = Convert.ToInt32(Console.ReadLine());

    Console.WriteLine("Введите число B: ");
    int userInput79 = Convert.ToInt32(Console.ReadLine());

    Console.WriteLine("Введите число C: ");
    int userInput80 = Convert.ToInt32(Console.ReadLine());

    if (userInput78 >= userInput79 && userInput78 >= userInput80)
        Console.WriteLine($"Максимум: {userInput78}");
    else if (userInput79 >= userInput78 && userInput79 >= userInput80)
        Console.WriteLine($"Максимум: {userInput79}");
    else
        Console.WriteLine($"Максимум: {userInput80}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 64. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program64
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Даны три числа. Найти минимальное из них.
               

    Console.WriteLine("Введите первое число: ");
    double userInput81 = Convert.ToDouble(Console.ReadLine());

    Console.WriteLine("Введите второе число: ");
    double userInput82 = Convert.ToDouble(Console.ReadLine());

    Console.WriteLine("Введите третье число: ");
    double userInput83 = Convert.ToDouble(Console.ReadLine());

    if (userInput81 <= userInput82 && userInput81 <= userInput83)
        Console.WriteLine($"Минимум: {userInput81}");
    else if (userInput82 <= userInput81 && userInput82 <= userInput83)
        Console.WriteLine($"Минимум: {userInput82}");
    else
        Console.WriteLine($"Минимум: {userInput83}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>







> ### Программа 65. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program65
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Даны три числа. Определить, сколько из них положительных (0, 1, 2 или 3).
               

    Console.WriteLine("Введите первое число: ");
    double userInput84 = Convert.ToDouble(Console.ReadLine());

    Console.WriteLine("Введите второе число: ");
    double userInput85 = Convert.ToDouble(Console.ReadLine());

    Console.WriteLine("Введите третье число: ");
    double userInput86 = Convert.ToDouble(Console.ReadLine());

    int count = 0;
    if (userInput84 > 0) count++;
    if (userInput85 > 0) count++;
    if (userInput86 > 0) count++;

    Console.WriteLine($"Положительных чисел: {count}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 66. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program66
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Ввести средний балл диплома. Вывести: «Без отличия» (<4.5), «Претендент на красный диплом» (4.5 - 4.74), «Красный диплом» (≥4.75).
 

     Console.WriteLine("Введите средний балл: ");
     double userInput87 = Convert.ToDouble(Console.ReadLine());

     if (userInput87 < 4.5)
         Console.WriteLine("Без отличия");
     else if (userInput87 < 4.75)
         Console.WriteLine("Претендент на красный диплом");
     else
         Console.WriteLine("Красный диплом");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 67. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program67
{
    internal class Program
    {
        static void Main(string[] args)
        {

  //Ввести значение артериального давления (систолическое). Вывести: гипотония (<90), норма(90 - 120), предгипертензия(121 - 139), гипертензия(≥140).
  

      Console.WriteLine("Введите систолическое давление: ");
      int userInput88 = Convert.ToInt32(Console.ReadLine());

      if (userInput88 < 90)
          Console.WriteLine("Гипотония");
      else if (userInput88 <= 120)
          Console.WriteLine("Норма");
      else if (userInput88 <= 139)
          Console.WriteLine("Предгипертензия");
      else
          Console.WriteLine("Гипертензия");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 68. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program68
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Ввести рейтинг шахматиста (Эло). Вывести ранг: любитель (<1400), разрядник(1400 - 1999), мастер(2000 - 2399), гроссмейстер(≥2400).


    Console.WriteLine("Введите рейтинг Эло: ");
    int userInput89 = Convert.ToInt32(Console.ReadLine());

    if (userInput89 < 1400)
        Console.WriteLine("Любитель");
    else if (userInput89 < 2000)
        Console.WriteLine("Разрядник");
    else if (userInput89 < 2400)
        Console.WriteLine("Мастер");
    else
        Console.WriteLine("Гроссмейстер");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 69. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program69
{
    internal class Program
    {
        static void Main(string[] args)
        {


                //Ввести число и определить, сколькизначным оно является (однозначное, двузначное, трехзначное или более).
               

                    Console.WriteLine("Введите целое число: ");
                    int userInput90 = Convert.ToInt32(Console.ReadLine());

                    int abs90 = Math.Abs(userInput90);

                    if (abs90 < 10)
                        Console.WriteLine("Однозначное");
                    else if (abs90 < 100)
                        Console.WriteLine("Двузначное");
                    else if (abs90 < 1000)
                        Console.WriteLine("Трехзначное");
                    else
                        Console.WriteLine("Более трех знаков");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 70. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program70
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Ввести дальность поездки на такси (км). Рассчитать тариф: до 5 км — 200 руб, от 5 до 15 км — 200 + 25 руб/км, свыше 15 км — 200 + 20 руб/км.
               

    Console.WriteLine("Введите дальность поездки (км): ");
    double userInput91 = Convert.ToDouble(Console.ReadLine());

    if (userInput91 <= 5)
        Console.WriteLine("Стоимость: 200 руб");
    else if (userInput91 <= 15)
        Console.WriteLine($"Стоимость: {200 + 25 * userInput91} руб");
    else
        Console.WriteLine($"Стоимость: {200 + 20 * userInput91} руб");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 71. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program71
{
    internal class Program
    {
        static void Main(string[] args)
        {


                //Ввести количество осадков за сутки (мм). Определить: без осадков (0), слабый дождь (0.1-4), умеренный (4.1-15), сильный ливень (>15).
              
                    Console.WriteLine("Введите количество осадков (мм): ");
                    double userInput92 = Convert.ToDouble(Console.ReadLine());

                    if (userInput92 == 0)
                        Console.WriteLine("Без осадков");
                    else if (userInput92 <= 4)
                        Console.WriteLine("Слабый дождь");
                    else if (userInput92 <= 15)
                        Console.WriteLine("Умеренный");
                    else
                        Console.WriteLine("Сильный ливень");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 72. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program72
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Ввести процент выполнения плана продаж. Вывести статус: план сорван (<70), удовлетворительно(70 - 99 %), выполнен(100 - 119 %), перевыполнен(≥120).


     

     Console.WriteLine("Введите процент выполнения плана: ");
     double userInput93 = Convert.ToDouble(Console.ReadLine());

     if (userInput93 < 70)
         Console.WriteLine("План сорван");
     else if (userInput93 < 100)
         Console.WriteLine("Удовлетворительно");
     else if (userInput93 < 120)
         Console.WriteLine("Выполнен");
     else
         Console.WriteLine("Перевыполнен");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 73. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program73
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Даны три числа. Упорядочить их по возрастанию и вывести на консоль.
 

     Console.WriteLine("Введите первое число: ");
     double userInput94 = Convert.ToDouble(Console.ReadLine());

     Console.WriteLine("Введите второе число: ");
     double userInput95 = Convert.ToDouble(Console.ReadLine());

     Console.WriteLine("Введите третье число: ");
     double userInput96 = Convert.ToDouble(Console.ReadLine());

     double temp94;
     if (userInput94 > userInput95)
     {
         temp94 = userInput94;
         userInput94 = userInput95;
         userInput95 = temp94;
     }
     if (userInput95 > userInput96)
     {
         temp94 = userInput95;
         userInput95 = userInput96;
         userInput96 = temp94;
     }
     if (userInput94 > userInput95)
     {
         temp94 = userInput94;
         userInput94 = userInput95;
         userInput95 = temp94;
     }

     Console.WriteLine($"По возрастанию: {userInput94}, {userInput95}, {userInput96}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 74. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program74
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Дано число X.Вычислить значение кусочно - заданной функции:f(x)=x2, еслиx>0;f(x)=0, еслиx=0;f(x)=−x, еслиx<0.


     Console.WriteLine("Введите число X: ");
     double userInput97 = Convert.ToDouble(Console.ReadLine());

     if (userInput97 > 0)
         Console.WriteLine($"f(x) = {userInput97 * userInput97}");
     else if (userInput97 == 0)
         Console.WriteLine("f(x) = 0");
     else
         Console.WriteLine($"f(x) = {-userInput97}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 75. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program75
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Ввести октановое число бензина. Классифицировать: <92 — несоответствие стандарту, 92 — АИ - 92, 95 — АИ - 95, 98 - 100 — АИ - 98 / 100, >100 — спорт / авиатопливо.


    Console.WriteLine("Введите октановое число: ");
    double userInput98 = Convert.ToDouble(Console.ReadLine());

    if (userInput98 < 92)
        Console.WriteLine("Несоответствие стандарту");
    else if (userInput98 == 92)
        Console.WriteLine("АИ-92");
    else if (userInput98 == 95)
        Console.WriteLine("АИ-95");
    else if (userInput98 <= 100)
        Console.WriteLine("АИ-98/100");
    else
        Console.WriteLine("Спорт/авиатопливо");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 76. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program76
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Ввести сумму покупок за месяц для начисления кешбэка: до 10 000 руб — 1%, до 50 000 руб — 3%, свыше 50 000 руб — 5%. Вывести сумму кешбэка.


     Console.WriteLine("Введите сумму покупок за месяц: ");
     double userInput99 = Convert.ToDouble(Console.ReadLine());

     if (userInput99 <= 10000)
         Console.WriteLine($"Кешбэк: {userInput99 * 0.01}");
     else if (userInput99 <= 50000)
         Console.WriteLine($"Кешбэк: {userInput99 * 0.03}");
     else
         Console.WriteLine($"Кешбэк: {userInput99 * 0.05}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 77. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program77
{
    internal class Program
    {
        static void Main(string[] args)
        {
   //Ввести глубину погружения аквалангиста (метры). Вывести зону: рекреационная (<40), техническая(40 - 100), глубоководная(>100).
  

       Console.WriteLine("Введите глубину погружения (м): ");
       double userInput100 = Convert.ToDouble(Console.ReadLine());

       if (userInput100 < 40)
           Console.WriteLine("Рекреационная зона");
       else if (userInput100 <= 100)
           Console.WriteLine("Техническая зона");
       else
           Console.WriteLine("Глубоководная зона");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 78. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program78
{
    internal class Program
    {
        static void Main(string[] args)
        {
    //Ввести количество штрафных баллов водителя. Вывести: «Предупреждение» (1-5), «Временное ограничение» (6-10), «Лишение прав» (>10).
   

        Console.WriteLine("Введите количество штрафных баллов: ");
        int userInput101 = Convert.ToInt32(Console.ReadLine());

        if (userInput101 <= 5)
            Console.WriteLine("Предупреждение");
        else if (userInput101 <= 10)
            Console.WriteLine("Временное ограничение");
        else
            Console.WriteLine("Лишение прав");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 79. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program79
{
    internal class Program
    {
        static void Main(string[] args)
        {

    //Ввести уровень кислотности почвы (pH). Определить: кислая (<6.0), нейтральная(6.0 - 7.2), щелочная(>7.2).
    

        Console.WriteLine("Введите уровень pH: ");
        double userInput102 = Convert.ToDouble(Console.ReadLine());

        if (userInput102 < 6.0)
            Console.WriteLine("Кислая");
        else if (userInput102 <= 7.2)
            Console.WriteLine("Нейтральная");
        else
            Console.WriteLine("Щелочная");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 80. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program80
{
    internal class Program
    {
        static void Main(string[] args)
        {


                //Ввести количество набранных очков в компьютерной игре. Присвоить медаль: Бронзовая (1000-2499), Серебряная (2500-4999), Золотая (5000+), иначе без медали.
               
                    Console.WriteLine("Введите количество очков: ");
                    int userInput103 = Convert.ToInt32(Console.ReadLine());

                    if (userInput103 < 1000)
                        Console.WriteLine("Без медали");
                    else if (userInput103 < 2500)
                        Console.WriteLine("Бронзовая медаль");
                    else if (userInput103 < 5000)
                        Console.WriteLine("Серебряная медаль");
                    else
                        Console.WriteLine("Золотая медаль");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 81. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program81
{
    internal class Program
    {
        static void Main(string[] args)
        {

       //Ввести крепость напитка в градусах. Классифицировать: безалкогольный (0), слабоалкогольный (0.1-8), среднеалкогольный (8.1-25), крепкий (>25).


           Console.WriteLine("Введите крепость напитка (градусы): ");
           double userInput104 = Convert.ToDouble(Console.ReadLine());

           if (userInput104 == 0)
               Console.WriteLine("Безалкогольный");
           else if (userInput104 <= 8)
               Console.WriteLine("Слабоалкогольный");
           else if (userInput104 <= 25)
               Console.WriteLine("Среднеалкогольный");
           else
               Console.WriteLine("Крепкий");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 82. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program82
{
    internal class Program
    {
        static void Main(string[] args)
        {
   //Ввести показатель уровня шума в децибелах (дБ). Вывести вердикт: тихо (<40), норма(40 - 60), шумно(61 - 80), вредно для здоровья(>80).


       Console.WriteLine("Введите уровень шума (дБ): ");
       double userInput105 = Convert.ToDouble(Console.ReadLine());

       if (userInput105 < 40)
           Console.WriteLine("Тихо");
       else if (userInput105 <= 60)
           Console.WriteLine("Норма");
       else if (userInput105 <= 80)
           Console.WriteLine("Шумно");
       else
           Console.WriteLine("Вредно для здоровья");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 83. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program83
{
    internal class Program
    {
        static void Main(string[] args)
        {

    //Ввести вес почтовой посылки (кг). Рассчитать категорию отправления: мелкий пакет (<2), стандартная(2 - 10), тяжеловесная(10.1 - 31.5), крупногабарит(>31.5).
   

        Console.WriteLine("Введите вес посылки (кг): ");
        double userInput106 = Convert.ToDouble(Console.ReadLine());

        if (userInput106 < 2)
            Console.WriteLine("Мелкий пакет");
        else if (userInput106 <= 10)
            Console.WriteLine("Стандартная");
        else if (userInput106 <= 31.5)
            Console.WriteLine("Тяжеловесная");
        else
            Console.WriteLine("Крупногабарит");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 84. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program84
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Ввести количество комнат в квартире. Вывести: студия/однокомнатная (1), двухкомнатная (2), трехкомнатная (3), многокомнатная (4+).
 

     Console.WriteLine("Введите количество комнат: ");
     int userInput107 = Convert.ToInt32(Console.ReadLine());

     if (userInput107 == 1)
         Console.WriteLine("Студия/однокомнатная");
     else if (userInput107 == 2)
         Console.WriteLine("Двухкомнатная");
     else if (userInput107 == 3)
         Console.WriteLine("Трехкомнатная");
     else
         Console.WriteLine("Многокомнатная");


        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 85. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program85
{
    internal class Program
    {
        static void Main(string[] args)
        {

   //Ввести процент заряда повербанка. Вывести количество светящихся светодиодов на корпусе (1, 2, 3 или 4).


       Console.WriteLine("Введите процент заряда повербанка: ");
       int userInput108 = Convert.ToInt32(Console.ReadLine());

       if (userInput108 <= 25)
           Console.WriteLine("Светится 1 светодиод");
       else if (userInput108 <= 50)
           Console.WriteLine("Светится 2 светодиода");
       else if (userInput108 <= 75)
           Console.WriteLine("Светится 3 светодиода");
       else
           Console.WriteLine("Светится 4 светодиода");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 86. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program86
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Ввести выслугу лет военнослужащего. Вывести процент пенсионной надбавки.
 

     Console.WriteLine("Введите выслугу лет: ");
     int userInput109 = Convert.ToInt32(Console.ReadLine());

     if (userInput109 < 5)
         Console.WriteLine("Надбавка: 0%");
     else if (userInput109 < 10)
         Console.WriteLine("Надбавка: 10%");
     else if (userInput109 < 15)
         Console.WriteLine("Надбавка: 20%");
     else if (userInput109 < 20)
         Console.WriteLine("Надбавка: 30%");
     else
         Console.WriteLine("Надбавка: 40%");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 87. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program87
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Ввести время отклика сервера (пинг в мс). Вывести: идеальный (<20), хороший(20 - 60), посредственный(61 - 120), плохой(>120).
 

     Console.WriteLine("Введите пинг (мс): ");
     int userInput110 = Convert.ToInt32(Console.ReadLine());

     if (userInput110 < 20)
         Console.WriteLine("Идеальный");
     else if (userInput110 <= 60)
         Console.WriteLine("Хороший");
     else if (userInput110 <= 120)
         Console.WriteLine("Посредственный");
     else
         Console.WriteLine("Плохой");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 88. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program88
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Ввести концентрацию CO2 в помещении (ppm). Вывести вердикт: норма (<800), душно(800 - 1200), проветрить немедленно(>1200).


     Console.WriteLine("Введите концентрацию CO2 (ppm): ");
     int userInput111 = Convert.ToInt32(Console.ReadLine());

     if (userInput111 < 800)
         Console.WriteLine("Норма");
     else if (userInput111 <= 1200)
         Console.WriteLine("Душно");
     else
         Console.WriteLine("Проветрить немедленно");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 89. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program89
{
    internal class Program
    {
        static void Main(string[] args)
        {
    //Ввести количество пройденных шагов за день. Вывести: гиподинамия (<5000), норма(5000 - 9999), активный день(10000 - 14999), рекорд(>15000).
    

        Console.WriteLine("Введите количество шагов: ");
        int userInput112 = Convert.ToInt32(Console.ReadLine());

        if (userInput112 < 5000)
            Console.WriteLine("Гиподинамия");
        else if (userInput112 < 10000)
            Console.WriteLine("Норма");
        else if (userInput112 < 15000)
            Console.WriteLine("Активный день");
        else
            Console.WriteLine("Рекорд");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 90. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program90
{
    internal class Program
    {
        static void Main(string[] args)
        {
  //Ввести диаметр автомобильного колесного диска в дюймах. Определить класс: малолитражки (13-14), компактные авто (15-16), кроссоверы/бизнес (17-19), внедорожники/спорт (20+).
 

      Console.WriteLine("Введите диаметр диска (дюймы): ");
      int userInput113 = Convert.ToInt32(Console.ReadLine());

      if (userInput113 <= 14)
          Console.WriteLine("Малолитражки");
      else if (userInput113 <= 16)
          Console.WriteLine("Компактные авто");
      else if (userInput113 <= 19)
          Console.WriteLine("Кроссоверы/бизнес");
      else
          Console.WriteLine("Внедорожники/спорт");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 91. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program91
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Ввести значение влажности воздуха (%). Вывести: сухой воздух (<30), комфорт(30 - 60), повышенная влажность(>60).


     Console.WriteLine("Введите влажность (%): ");
     double userInput114 = Convert.ToDouble(Console.ReadLine());

     if (userInput114 < 30)
         Console.WriteLine("Сухой воздух");
     else if (userInput114 <= 60)
         Console.WriteLine("Комфорт");
     else
         Console.WriteLine("Повышенная влажность");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 92. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program92
{
    internal class Program
    {
        static void Main(string[] args)
        {
    //Даны три числа. Проверить, сколько из них равны между собой (все разные, два равны, все три равны).
  

        Console.WriteLine("Введите первое число: ");
        double userInput115 = Convert.ToDouble(Console.ReadLine());

        Console.WriteLine("Введите второе число: ");
        double userInput116 = Convert.ToDouble(Console.ReadLine());

        Console.WriteLine("Введите третье число: ");
        double userInput117 = Convert.ToDouble(Console.ReadLine());

        if (userInput115 == userInput116 && userInput116 == userInput117)
            Console.WriteLine("Все три числа равны");
        else if (userInput115 == userInput116 || userInput115 == userInput117 || userInput116 == userInput117)
            Console.WriteLine("Два числа равны");
        else
            Console.WriteLine("Все числа разные");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 93. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program93
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Ввести номер четверти координатной плоскости (1–4) и вывести диапазоны знаков для координат X и Y.


    Console.WriteLine("Введите номер четверти (1–4): ");
    int userInput118 = Convert.ToInt32(Console.ReadLine());

    if (userInput118 == 1)
        Console.WriteLine("X > 0, Y > 0");
    else if (userInput118 == 2)
        Console.WriteLine("X < 0, Y > 0");
    else if (userInput118 == 3)
        Console.WriteLine("X < 0, Y < 0");
    else if (userInput118 == 4)
        Console.WriteLine("X > 0, Y < 0");
    else
        Console.WriteLine("Некорректный номер четверти");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 94. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program94
{
    internal class Program
    {
        static void Main(string[] args)
        {

                //Ввести температуру процессора компьютера. Вывести: холодный (<45), нормальная нагрузка(45 - 75), троттлинг / перегрев(>75).
                

                    Console.WriteLine("Введите температуру процессора (°C): ");
                    double userInput119 = Convert.ToDouble(Console.ReadLine());

                    if (userInput119 < 45)
                        Console.WriteLine("Холодный");
                    else if (userInput119 <= 75)
                        Console.WriteLine("Нормальная нагрузка");
                    else
                        Console.WriteLine("Троттлинг/перегрев");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 95. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program95
{
    internal class Program
    {
        static void Main(string[] args)
        {
 //Ввести остаток срока годности продукта в днях. Вывести: «Срочно употребить» (≤2), «Нормально» (3 - 30), «Длительное хранение» (>30).


     Console.WriteLine("Введите остаток срока годности (дней): ");
     int userInput120 = Convert.ToInt32(Console.ReadLine());

     if (userInput120 <= 2)
         Console.WriteLine("Срочно употребить");
     else if (userInput120 <= 30)
         Console.WriteLine("Нормально");
     else
         Console.WriteLine("Длительное хранение");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 96. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program96
{
    internal class Program
    {
        static void Main(string[] args)
        {

 //Ввести сумму кредита и срок. Рассчитать процентную ставку в зависимости от срока (до года, до трех лет, свыше трех лет).


     Console.WriteLine("Введите сумму кредита: ");
     double userInput121 = Convert.ToDouble(Console.ReadLine());

     Console.WriteLine("Введите срок кредита (лет): ");
     double userInput122 = Convert.ToDouble(Console.ReadLine());

     if (userInput122 < 1)
         Console.WriteLine("Ставка: 15%");
     else if (userInput122 <= 3)
         Console.WriteLine("Ставка: 12%");
     else
         Console.WriteLine("Ставка: 10%");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 97. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program97
{
    internal class Program
    {
        static void Main(string[] args)
        {
  //Ввести частоту обновления монитора (Гц). Определить: офис (60-75), базовый игровой (120-144), киберспорт (165+).


      Console.WriteLine("Введите частоту обновления (Гц): ");
      int userInput123 = Convert.ToInt32(Console.ReadLine());

      if (userInput123 <= 75)
          Console.WriteLine("Офис");
      else if (userInput123 <= 144)
          Console.WriteLine("Базовый игровой");
      else
          Console.WriteLine("Киберспорт");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 98. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program98
{
    internal class Program
    {
        static void Main(string[] args)
        {

  //Ввести расход топлива автомобиля на 100 км пути. Вывести вердикт: экономичный (<6 л), средний(6 - 10 л), прожорливый(>10 л).
 

      Console.WriteLine("Введите расход топлива (л/100 км): ");
      double userInput124 = Convert.ToDouble(Console.ReadLine());

      if (userInput124 < 6)
          Console.WriteLine("Экономичный");
      else if (userInput124 <= 10)
          Console.WriteLine("Средний");
      else
          Console.WriteLine("Прожорливый");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 99. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program99
{
    internal class Program
    {
        static void Main(string[] args)
        {
        //Ввести количество страниц книги. Классифицировать: брошюра (<48), повесть(48 - 150), роман(151 - 600), фолиант(>600).
       

            Console.WriteLine("Введите количество страниц: ");
            int userInput125 = Convert.ToInt32(Console.ReadLine());

            if (userInput125 < 48)
                Console.WriteLine("Брошюра");
            else if (userInput125 <= 150)
                Console.WriteLine("Повесть");
            else if (userInput125 <= 600)
                Console.WriteLine("Роман");
            else
                Console.WriteLine("Фолиант");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 100. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program100
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Ввести число и проверить, попадает ли оно в интервалы [0;10], [20;30] или [50;100].Ввести число и проверить, попадает ли оно в интервалы [0;10], [20;30] или [50;100].


    Console.WriteLine("Введите число: ");
    double userInput126 = Convert.ToDouble(Console.ReadLine());

    if (userInput126 >= 0 && userInput126 <= 10)
        Console.WriteLine("Число в интервале [0;10]");
    else if (userInput126 >= 20 && userInput126 <= 30)
        Console.WriteLine("Число в интервале [20;30]");
    else if (userInput126 >= 50 && userInput126 <= 100)
        Console.WriteLine("Число в интервале [50;100]");
    else
        Console.WriteLine("Число не попадает ни в один из интервалов");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

## Раздел 3. Составные логические условия &&, ||, !



> ### Программа 101. 


```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program101
{
    internal class Program
    {
        static void Main(string[] args)
        {
          //Задача 1. Дано целое число. Проверить, принадлежит ли оно числовому отрезку [10;50].
int userInput127 = Convert.ToInt32(Console.ReadLine());
if (userInput127 >= 10 && userInput127 <= 50)
    Console.WriteLine("Принадлежит отрезку [10;50]");
else
    Console.WriteLine("Не принадлежит отрезку [10;50]");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 102. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program102
{
    internal class Program
    {
        static void Main(string[] args)
        {
           //Задача 2. Проверить, является ли введенное целое число положительным и четным одновременно.
int userInput128 = Convert.ToInt32(Console.ReadLine());
if (userInput128 > 0 && userInput128 % 2 == 0)
    Console.WriteLine("Положительное и четное одновременно");
else
    Console.WriteLine("Не является положительным и четным одновременно");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 103. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program103
{
    internal class Program
    {
        static void Main(string[] args)
        {
          //Задача 3. Проверить, лежит ли число вне диапазона [-10;10].
int userInput129 = Convert.ToInt32(Console.ReadLine());
if (userInput129 < -10 || userInput129 > 10)
    Console.WriteLine("Число вне диапазона [-10;10]");
else
    Console.WriteLine("Число внутри диапазона [-10;10]");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 104. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program104
{
    internal class Program
    {
        static void Main(string[] args)
        {
        //Задача 4. Ввести логин и пароль пользователя. Вывести «Успех», если логин равен admin и пароль secret.
string userInput130 = Console.ReadLine();
string userInput131 = Console.ReadLine();
if (userInput130 == "admin" && userInput131 == "secret")
    Console.WriteLine("Успех");
else
    Console.WriteLine("Неверный логин или пароль");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 105. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program105
{
    internal class Program
    {
        static void Main(string[] args)
        {
         //Задача 5. Проверить, является ли введенный год високосным (делится на 4, но не на 100, либо делится на 400).
int userInput132 = Convert.ToInt32(Console.ReadLine());
if ((userInput132 % 4 == 0 && userInput132 % 100 != 0) || userInput132 % 400 == 0)
    Console.WriteLine("Високосный");
else
    Console.WriteLine("Не високосный");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>
---





> ### Программа 106. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program106
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 6. Даны координаты точки (X, Y). Определить, попадает ли точка в I координатную четверть (X > 0 и Y > 0).
double userInput133 = Convert.ToDouble(Console.ReadLine());
double userInput134 = Convert.ToDouble(Console.ReadLine());
if (userInput133 > 0 && userInput134 > 0)
    Console.WriteLine("I четверть");
else
    Console.WriteLine("Не I четверть");
        }
    }
}
        
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 107. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program107
{
    internal class Program
    {
        static void Main(string[] args)
        {
        //Задача 7. Определить, попадает ли точка (X, Y) во II четверть плоскости.
double userInput135 = Convert.ToDouble(Console.ReadLine());
double userInput136 = Convert.ToDouble(Console.ReadLine());
if (userInput135 < 0 && userInput136 > 0)
    Console.WriteLine("II четверть");
else
    Console.WriteLine("Не II четверть");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 108. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program108
{
    internal class Program
    {
        static void Main(string[] args)
        {
         //Задача 8. Определить, попадает ли точка (X, Y) в III четверть плоскости.
double userInput137 = Convert.ToDouble(Console.ReadLine());
double userInput138 = Convert.ToDouble(Console.ReadLine());
if (userInput137 < 0 && userInput138 < 0)
    Console.WriteLine("III четверть");
else
    Console.WriteLine("Не III четверть");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 109. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program109
{
    internal class Program
    {
        static void Main(string[] args)
        {
           //Задача 9. Определить, попадает ли точка (X, Y) в IV четверть плоскости.
double userInput139 = Convert.ToDouble(Console.ReadLine());
double userInput140 = Convert.ToDouble(Console.ReadLine());
if (userInput139 > 0 && userInput140 < 0)
    Console.WriteLine("IV четверть");
else
    Console.WriteLine("Не IV четверть");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 110. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program110
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 10. Даны три стороны A, B, C. Проверить, является ли треугольник прямоугольным (теорема Пифагора).
double userInput141 = Convert.ToDouble(Console.ReadLine());
double userInput142 = Convert.ToDouble(Console.ReadLine());
double userInput143 = Convert.ToDouble(Console.ReadLine());
if (userInput141 * userInput141 + userInput142 * userInput142 == userInput143 * userInput143 ||
    userInput141 * userInput141 + userInput143 * userInput143 == userInput142 * userInput142 ||
    userInput142 * userInput142 + userInput143 * userInput143 == userInput141 * userInput141)
    Console.WriteLine("Прямоугольный");
else
    Console.WriteLine("Не прямоугольный");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 111. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program111
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 11. Даны три стороны. Проверить, является ли треугольник равнобедренным.
double userInput144 = Convert.ToDouble(Console.ReadLine());
double userInput145 = Convert.ToDouble(Console.ReadLine());
double userInput146 = Convert.ToDouble(Console.ReadLine());
if (userInput144 == userInput145 || userInput144 == userInput146 || userInput145 == userInput146)
    Console.WriteLine("Равнобедренный");
else
    Console.WriteLine("Не равнобедренный");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>








> ### Программа 112. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program112
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 12. Ввести возраст и стаж вождения. Разрешить аренду каршеринга бизнес-класса, если возраст ≥ 23 лет И стаж ≥ 3 лет.
int userInput147 = Convert.ToInt32(Console.ReadLine());
int userInput148 = Convert.ToInt32(Console.ReadLine());
if (userInput147 >= 23 && userInput148 >= 3)
    Console.WriteLine("Аренда разрешена");
else
    Console.WriteLine("Аренда запрещена");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 113. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program113
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 13. Проверить, делится ли число одновременно на 3 и на 5 без остатка.
int userInput149 = Convert.ToInt32(Console.ReadLine());
if (userInput149 % 3 == 0 && userInput149 % 5 == 0)
    Console.WriteLine("Делится на 3 и на 5");
else
    Console.WriteLine("Не делится на 3 и на 5 одновременно");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 114. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program114
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 14. Проверить, является ли число трехзначным и оканчивается ли оно на цифру 5.
int userInput150 = Convert.ToInt32(Console.ReadLine());
if (userInput150 >= 100 && userInput150 <= 999 && userInput150 % 10 == 5)
    Console.WriteLine("Трехзначное и оканчивается на 5");
else
    Console.WriteLine("Не подходит");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>







> ### Программа 115. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program115
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 15. Даны три числа. Проверить, упорядочены ли они строго по возрастанию (A < B < C).
double userInput151 = Convert.ToDouble(Console.ReadLine());
double userInput152 = Convert.ToDouble(Console.ReadLine());
double userInput153 = Convert.ToDouble(Console.ReadLine());
if (userInput151 < userInput152 && userInput152 < userInput153)
    Console.WriteLine("Строго по возрастанию");
else
    Console.WriteLine("Не по возрастанию");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 116. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program116
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 16. Проверить, верно ли, что среди трех введенных чисел есть хотя бы одно четное.
int userInput154 = Convert.ToInt32(Console.ReadLine());
int userInput155 = Convert.ToInt32(Console.ReadLine());
int userInput156 = Convert.ToInt32(Console.ReadLine());
if (userInput154 % 2 == 0 || userInput155 % 2 == 0 || userInput156 % 2 == 0)
    Console.WriteLine("Есть хотя бы одно четное");
else
    Console.WriteLine("Нет четных");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 117. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program117
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 17. Проверить, верно ли, что среди трех чисел ровно одно равно нулю.
double userInput157 = Convert.ToDouble(Console.ReadLine());
double userInput158 = Convert.ToDouble(Console.ReadLine());
double userInput159 = Convert.ToDouble(Console.ReadLine());
int userInput160 = 0;
if (userInput157 == 0) userInput160++;
if (userInput158 == 0) userInput160++;
if (userInput159 == 0) userInput160++;
if (userInput160 == 1)
    Console.WriteLine("Ровно одно равно нулю");
else
    Console.WriteLine("Не ровно одно равно нулю");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 118. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program118
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 18. Ввести температуру и влажность. Вывести предупреждение о гололедице, если температура ≤ 0 °C И влажность > 85.
double userInput161 = Convert.ToDouble(Console.ReadLine());
double userInput162 = Convert.ToDouble(Console.ReadLine());
if (userInput161 <= 0 && userInput162 > 85)
    Console.WriteLine("Гололедица!");
else
    Console.WriteLine("Гололедицы нет");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 119. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program119
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 19. Даны координаты точки (X, Y). Проверить, лежит ли точка внутри круга радиуса R с центром в начале координат (x^2 + y^2 ≤ R^2).
double userInput163 = Convert.ToDouble(Console.ReadLine());
double userInput164 = Convert.ToDouble(Console.ReadLine());
double userInput165 = Convert.ToDouble(Console.ReadLine());
if (userInput163 * userInput163 + userInput164 * userInput164 <= userInput165 * userInput165)
    Console.WriteLine("Внутри круга");
else
    Console.WriteLine("Вне круга");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 120. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program120
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 20. Даны координаты точки (X, Y). Проверить, лежит ли точка внутри прямоугольника со сторонами, параллельными осям, заданного углами (X1, Y1) и (X2, Y2).
double userInput166 = Convert.ToDouble(Console.ReadLine());
double userInput167 = Convert.ToDouble(Console.ReadLine());
double userInput168 = Convert.ToDouble(Console.ReadLine());
double userInput169 = Convert.ToDouble(Console.ReadLine());
double userInput170 = Convert.ToDouble(Console.ReadLine());
double userInput171 = Convert.ToDouble(Console.ReadLine());
double userInput172 = Math.Min(userInput168, userInput170);
double userInput173 = Math.Max(userInput168, userInput170);
double userInput174 = Math.Min(userInput169, userInput171);
double userInput175 = Math.Max(userInput169, userInput171);
if (userInput166 >= userInput172 && userInput166 <= userInput173 && userInput167 >= userInput174 && userInput167 <= userInput175)
    Console.WriteLine("Внутри прямоугольника");
else
    Console.WriteLine("Вне прямоугольника");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 121. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program121
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 21. Ввести день и месяц рождения. Проверить, корректна ли дата (например, день от 1 до 31, месяц от 1 до 12, с учетом длины месяцев).
int userInput176 = Convert.ToInt32(Console.ReadLine());
int userInput177 = Convert.ToInt32(Console.ReadLine());
bool userInput178 = false;
if (userInput177 >= 1 && userInput177 <= 12 && userInput176 >= 1)
{
    if (userInput177 == 2) userInput178 = userInput176 <= 28;
    else if (userInput177 == 4 || userInput177 == 6 || userInput177 == 9 || userInput177 == 11) userInput178 = userInput176 <= 30;
    else userInput178 = userInput176 <= 31;
}
Console.WriteLine(userInput178 ? "Дата корректна" : "Дата некорректна");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 122. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program122
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 22. Ввести номер месяца. Проверить, относится ли он к зимнему периоду (12, 1 или 2).
int userInput179 = Convert.ToInt32(Console.ReadLine());
if (userInput179 == 12 || userInput179 == 1 || userInput179 == 2)
    Console.WriteLine("Зимний месяц");
else
    Console.WriteLine("Не зимний месяц");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 123. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program123
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 23. Проверить, является ли четырехзначное число «счастливым билетом» (сумма первых двух цифр равна сумме двух последних).
int userInput180 = Convert.ToInt32(Console.ReadLine());
if (userInput180 >= 1000 && userInput180 <= 9999)
{
    int userInput181 = userInput180 / 1000;
    int userInput182 = (userInput180 / 100) % 10;
    int userInput183 = (userInput180 / 10) % 10;
    int userInput184 = userInput180 % 10;
    if (userInput181 + userInput182 == userInput183 + userInput184)
        Console.WriteLine("Счастливый билет");
    else
        Console.WriteLine("Не счастливый билет");
}
else
    Console.WriteLine("Не четырехзначное");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 124. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program124
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 24. Ввести три числа. Проверить истинность высказывания: «Хотя бы одна пара чисел взаимно противоположна (A = -B)».
double userInput185 = Convert.ToDouble(Console.ReadLine());
double userInput186 = Convert.ToDouble(Console.ReadLine());
double userInput187 = Convert.ToDouble(Console.ReadLine());
if (userInput185 == -userInput186 || userInput185 == -userInput187 || userInput186 == -userInput187)
    Console.WriteLine("Есть взаимно противоположная пара");
else
    Console.WriteLine("Нет взаимно противоположной пары");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 125. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program125
{
    internal class Program
    {
        static void Main(string[] args)
        {


//Задача 25. Пользователь вводит показания двух датчиков аварии. Сформировать тревогу, если сработал хотя бы один датчик И при этом включен тумблер защиты.
bool userInput188 = Convert.ToBoolean(Console.ReadLine());
bool userInput189 = Convert.ToBoolean(Console.ReadLine());
bool userInput190 = Convert.ToBoolean(Console.ReadLine());
if ((userInput188 || userInput189) && userInput190)
    Console.WriteLine("ТРЕВОГА!");
else
    Console.WriteLine("Тревоги нет");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 126. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program126
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 26. Проверить, лежит ли число X строго между числами A и B (учесть, что A может быть больше B).
double userInput191 = Convert.ToDouble(Console.ReadLine());
double userInput192 = Convert.ToDouble(Console.ReadLine());
double userInput193 = Convert.ToDouble(Console.ReadLine());
double userInput194 = Math.Min(userInput192, userInput193);
double userInput195 = Math.Max(userInput192, userInput193);
if (userInput191 > userInput194 && userInput191 < userInput195)
    Console.WriteLine("X строго между A и B");
else
    Console.WriteLine("X не между A и B");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 127. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program127
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 27. Даны два целых числа. Проверить, имеют ли они одинаковый знак (оба положительные или оба отрицательные).
int userInput196 = Convert.ToInt32(Console.ReadLine());
int userInput197 = Convert.ToInt32(Console.ReadLine());
if ((userInput196 > 0 && userInput197 > 0) || (userInput196 < 0 && userInput197 < 0))
    Console.WriteLine("Одинаковый знак");
else
    Console.WriteLine("Разный знак");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 128. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program128
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 28. Даны шахматные координаты двух клеток (x1, y1) и (x2, y2) от 1 до 8. Определить, угрожает ли ладья с первой клетки фигуре на второй клетке (совпадает либо строка, либо столбец).
int userInput198 = Convert.ToInt32(Console.ReadLine());
int userInput199 = Convert.ToInt32(Console.ReadLine());
int userInput200 = Convert.ToInt32(Console.ReadLine());
int userInput201 = Convert.ToInt32(Console.ReadLine());
if (userInput198 == userInput200 || userInput199 == userInput201)
    Console.WriteLine("Ладья угрожает");
else
    Console.WriteLine("Ладья не угрожает");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 129. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program129
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 29. Для двух клеток шахматной доски определить, угрожает ли слон (разность координат по модулю одинакова).
int userInput202 = Convert.ToInt32(Console.ReadLine());
int userInput203 = Convert.ToInt32(Console.ReadLine());
int userInput204 = Convert.ToInt32(Console.ReadLine());
int userInput205 = Convert.ToInt32(Console.ReadLine());
if (Math.Abs(userInput202 - userInput204) == Math.Abs(userInput203 - userInput205))
    Console.WriteLine("Слон угрожает");
else
    Console.WriteLine("Слон не угрожает");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 130. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program130
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 30. Для двух клеток шахматной доски определить, угрожает ли ферзь (объединение логики ладьи и слона).
int userInput206 = Convert.ToInt32(Console.ReadLine());
int userInput207 = Convert.ToInt32(Console.ReadLine());
int userInput208 = Convert.ToInt32(Console.ReadLine());
int userInput209 = Convert.ToInt32(Console.ReadLine());
if (userInput206 == userInput208 || userInput207 == userInput209 ||
    Math.Abs(userInput206 - userInput208) == Math.Abs(userInput207 - userInput209))
    Console.WriteLine("Ферзь угрожает");
else
    Console.WriteLine("Ферзь не угрожает");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 131. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program131
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 31. Для двух клеток определить, может ли конь пойти с одной на другую.
int userInput210 = Convert.ToInt32(Console.ReadLine());
int userInput211 = Convert.ToInt32(Console.ReadLine());
int userInput212 = Convert.ToInt32(Console.ReadLine());
int userInput213 = Convert.ToInt32(Console.ReadLine());
int userInput214 = Math.Abs(userInput210 - userInput212);
int userInput215 = Math.Abs(userInput211 - userInput213);
if ((userInput214 == 2 && userInput215 == 1) || (userInput214 == 1 && userInput215 == 2))
    Console.WriteLine("Конь может пойти");
else
    Console.WriteLine("Конь не может пойти");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 132. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program132
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 32. Для двух клеток шахматной доски проверить, одинакового ли они цвета.
int userInput216 = Convert.ToInt32(Console.ReadLine());
int userInput217 = Convert.ToInt32(Console.ReadLine());
int userInput218 = Convert.ToInt32(Console.ReadLine());
int userInput219 = Convert.ToInt32(Console.ReadLine());
if ((userInput216 + userInput217) % 2 == (userInput218 + userInput219) % 2)
    Console.WriteLine("Одинаковый цвет");
else
    Console.WriteLine("Разный цвет");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 133. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program133
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 33. Ввести рост и вес кандидата в космонавты. Проверить соответствие: рост от 160 до 190 см И вес от 50 до 90 кг.
int userInput220 = Convert.ToInt32(Console.ReadLine());
int userInput221 = Convert.ToInt32(Console.ReadLine());
if (userInput220 >= 160 && userInput220 <= 190 && userInput221 >= 50 && userInput221 <= 90)
    Console.WriteLine("Соответствует");
else
    Console.WriteLine("Не соответствует");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 134. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program134
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 34. Дано натуральное число N. Проверить, является ли оно четным двузначным числом.
int userInput222 = Convert.ToInt32(Console.ReadLine());
if (userInput222 >= 10 && userInput222 <= 99 && userInput222 % 2 == 0)
    Console.WriteLine("Четное двузначное");
else
    Console.WriteLine("Не четное двузначное");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 135. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program135
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 35. Дано натуральное число. Проверить, является ли оно нечетным трехзначным числом.
int userInput223 = Convert.ToInt32(Console.ReadLine());
if (userInput223 >= 100 && userInput223 <= 999 && userInput223 % 2 != 0)
    Console.WriteLine("Нечетное трехзначное");
else
    Console.WriteLine("Не нечетное трехзначное");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 136. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program136
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 36. Ввести результаты двух экзаменов (математика и информатика). Абитуриент зачислен, если сумма баллов ≥ 150 И по каждому предмету не менее 50 баллов.
int userInput224 = Convert.ToInt32(Console.ReadLine());
int userInput225 = Convert.ToInt32(Console.ReadLine());
if (userInput224 + userInput225 >= 150 && userInput224 >= 50 && userInput225 >= 50)
    Console.WriteLine("Зачислен");
else
    Console.WriteLine("Не зачислен");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 137. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program137
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 37. Проверить, лежит ли точка с координатами (X, Y) в круговом кольце с внутренним радиусом R1 и внешним R2.
double userInput226 = Convert.ToDouble(Console.ReadLine());
double userInput227 = Convert.ToDouble(Console.ReadLine());
double userInput228 = Convert.ToDouble(Console.ReadLine());
double userInput229 = Convert.ToDouble(Console.ReadLine());
double userInput230 = userInput226 * userInput226 + userInput227 * userInput227;
if (userInput230 >= userInput228 * userInput228 && userInput230 <= userInput229 * userInput229)
    Console.WriteLine("В кольце");
else
    Console.WriteLine("Не в кольце");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 138. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program138
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 38. Ввести статус билета (true/false) и наличие багажа. Вывести: требуется ли дополнительная оплата багажа.
bool userInput231 = Convert.ToBoolean(Console.ReadLine());
bool userInput232 = Convert.ToBoolean(Console.ReadLine());
if (userInput231 && userInput232)
    Console.WriteLine("Требуется доплата за багаж");
else
    Console.WriteLine("Доплата не требуется");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 139. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program139
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 39. Дано четырехзначное число. Проверить, читается ли оно одинаково слева направо и справа налево (палиндром).
int userInput233 = Convert.ToInt32(Console.ReadLine());
if (userInput233 >= 1000 && userInput233 <= 9999)
{
    int userInput234 = userInput233 / 1000;
    int userInput235 = (userInput233 / 100) % 10;
    int userInput236 = (userInput233 / 10) % 10;
    int userInput237 = userInput233 % 10;
    if (userInput234 == userInput237 && userInput235 == userInput236)
        Console.WriteLine("Палиндром");
    else
        Console.WriteLine("Не палиндром");
}
else
    Console.WriteLine("Не четырехзначное");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 140. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program140
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 40. Ввести напряжение сети (Вольты) и частоту (Гц). Норма: 220 В ± 10 И частота 50 Гц ± 1 Гц. Вывести статус стабильности сети.
double userInput238 = Convert.ToDouble(Console.ReadLine());
double userInput239 = Convert.ToDouble(Console.ReadLine());
if (userInput238 >= 210 && userInput238 <= 230 && userInput239 >= 49 && userInput239 <= 51)
    Console.WriteLine("Сеть стабильна");
else
    Console.WriteLine("Сеть нестабильна");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 141. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program141
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 41. Ввести признак наличия прав (bool), страховки (bool) и трезвости водителя (bool). Разрешить выезд только при соблюдении всех трех факторов.
bool userInput240 = Convert.ToBoolean(Console.ReadLine());
bool userInput241 = Convert.ToBoolean(Console.ReadLine());
bool userInput242 = Convert.ToBoolean(Console.ReadLine());
if (userInput240 && userInput241 && userInput242)
    Console.WriteLine("Выезд разрешен");
else
    Console.WriteLine("Выезд запрещен");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 142. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program142
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 42. Проверить, делится ли введенное число на 4 ИЛИ на 7, но НЕ делится на 28.
int userInput243 = Convert.ToInt32(Console.ReadLine());
if ((userInput243 % 4 == 0 || userInput243 % 7 == 0) && userInput243 % 28 != 0)
    Console.WriteLine("Условие выполнено");
else
    Console.WriteLine("Условие не выполнено");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 143. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program143
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 43. Ввести текущий месяц и температуру. Вывести аномалию, если месяц летний (6, 7, 8), а температура ниже нуля.
int userInput244 = Convert.ToInt32(Console.ReadLine());
double userInput245 = Convert.ToDouble(Console.ReadLine());
if ((userInput244 == 6 || userInput244 == 7 || userInput244 == 8) && userInput245 < 0)
    Console.WriteLine("Аномалия!");
else
    Console.WriteLine("Аномалии нет");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 144. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program144
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 44. Даны три логические переменные A, B, C. Реализовать проверку формулы мажоритарного клапана: «Истинно, если хотя бы две из трех переменных истинны».
bool userInput246 = Convert.ToBoolean(Console.ReadLine());
bool userInput247 = Convert.ToBoolean(Console.ReadLine());
bool userInput248 = Convert.ToBoolean(Console.ReadLine());
if ((userInput246 && userInput247) || (userInput246 && userInput248) || (userInput247 && userInput248))
    Console.WriteLine("Истинно");
else
    Console.WriteLine("Ложно");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 145. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program145
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 45. Даны три вещественных числа. Проверить, могут ли они являться длинами сторон тупоугольного треугольника.
double userInput249 = Convert.ToDouble(Console.ReadLine());
double userInput250 = Convert.ToDouble(Console.ReadLine());
double userInput251 = Convert.ToDouble(Console.ReadLine());
if (userInput249 + userInput250 > userInput251 && userInput249 + userInput251 > userInput250 && userInput250 + userInput251 > userInput249)
{
    double userInput252 = Math.Max(userInput249, Math.Max(userInput250, userInput251));
    double userInput253 = userInput249 * userInput249 + userInput250 * userInput250 + userInput251 * userInput251 - userInput252 * userInput252;
    if (userInput253 < userInput252 * userInput252)
        Console.WriteLine("Тупоугольный");
    else
        Console.WriteLine("Не тупоугольный");
}
else
    Console.WriteLine("Не треугольник");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 146. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program146
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 46. Даны три вещественных числа. Проверить, могут ли они являться длинами сторон остроугольного треугольника.
double userInput254 = Convert.ToDouble(Console.ReadLine());
double userInput255 = Convert.ToDouble(Console.ReadLine());
double userInput256 = Convert.ToDouble(Console.ReadLine());
if (userInput254 + userInput255 > userInput256 && userInput254 + userInput256 > userInput255 && userInput255 + userInput256 > userInput254)
{
    double userInput257 = Math.Max(userInput254, Math.Max(userInput255, userInput256));
    double userInput258 = userInput254 * userInput254 + userInput255 * userInput255 + userInput256 * userInput256 - userInput257 * userInput257;
    if (userInput258 > userInput257 * userInput257)
        Console.WriteLine("Остроугольный");
    else
        Console.WriteLine("Не остроугольный");
}
else
    Console.WriteLine("Не треугольник");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 147. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program147
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 47. Ввести время (часы и минуты). Проверить, попадает ли указанное время в интервал тихого часа (с 13:00 до 15:00).
int userInput259 = Convert.ToInt32(Console.ReadLine());
int userInput260 = Convert.ToInt32(Console.ReadLine());
int userInput261 = userInput259 * 60 + userInput260;
if (userInput261 >= 13 * 60 && userInput261 <= 15 * 60)
    Console.WriteLine("Тихий час");
else
    Console.WriteLine("Не тихий час");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 148. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program148
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 48. Проверить, что все цифры введенного трехзначного числа различны между собой.
int userInput262 = Convert.ToInt32(Console.ReadLine());
if (userInput262 >= 100 && userInput262 <= 999)
{
    int userInput263 = userInput262 / 100;
    int userInput264 = (userInput262 / 10) % 10;
    int userInput265 = userInput262 % 10;
    if (userInput263 != userInput264 && userInput263 != userInput265 && userInput264 != userInput265)
        Console.WriteLine("Все цифры различны");
    else
        Console.WriteLine("Есть одинаковые цифры");
}
else
    Console.WriteLine("Не трехзначное");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 149. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program149
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 49. Ввести логическое значение двух кнопок пульта. Станок запускается только при одновременном зажатии обеих кнопок (защита от случайного пуска).
bool userInput266 = Convert.ToBoolean(Console.ReadLine());
bool userInput267 = Convert.ToBoolean(Console.ReadLine());
if (userInput266 && userInput267)
    Console.WriteLine("Станок запущен");
else
    Console.WriteLine("Станок не запущен");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 150. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program150
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 50. Проверить, лежит ли точка (X, Y) ниже прямой Y = 2X + 1 и выше параболы Y = X^2.
double userInput268 = Convert.ToDouble(Console.ReadLine());
double userInput269 = Convert.ToDouble(Console.ReadLine());
if (userInput269 < 2 * userInput268 + 1 && userInput269 > userInput268 * userInput268)
    Console.WriteLine("Условие выполнено");
else
    Console.WriteLine("Условие не выполнено");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


## Раздел 2. Множественные ветвления else if и диапазоны

 ### Программа 151. 


```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program151
{
    internal class Program
    {
        static void Main(string[] args)
        {
          //Задача 51. Ввести номер дня недели (1–7). Вывести его словесное название на русском языке.
int userInput270 = Convert.ToInt32(Console.ReadLine());
switch (userInput270)
{
    case 1: Console.WriteLine("Понедельник"); break;
    case 2: Console.WriteLine("Вторник"); break;
    case 3: Console.WriteLine("Среда"); break;
    case 4: Console.WriteLine("Четверг"); break;
    case 5: Console.WriteLine("Пятница"); break;
    case 6: Console.WriteLine("Суббота"); break;
    case 7: Console.WriteLine("Воскресенье"); break;
    default: Console.WriteLine("Неверный номер"); break;
}
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 152. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program152
{
    internal class Program
    {
        static void Main(string[] args)
        {
           //Задача 52. Ввести номер дня недели (1–7). Вывести, является ли день рабочим («Будни») или нерабочим («Выходной»).
int userInput271 = Convert.ToInt32(Console.ReadLine());
switch (userInput271)
{
    case 1: case 2: case 3: case 4: case 5:
        Console.WriteLine("Будни"); break;
    case 6: case 7:
        Console.WriteLine("Выходной"); break;
    default: Console.WriteLine("Неверный номер"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 153. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program153
{
    internal class Program
    {
        static void Main(string[] args)
        {
          //Задача 53. Ввести номер месяца (1–12). Вывести название месяца.
int userInput272 = Convert.ToInt32(Console.ReadLine());
switch (userInput272)
{
    case 1: Console.WriteLine("Январь"); break;
    case 2: Console.WriteLine("Февраль"); break;
    case 3: Console.WriteLine("Март"); break;
    case 4: Console.WriteLine("Апрель"); break;
    case 5: Console.WriteLine("Май"); break;
    case 6: Console.WriteLine("Июнь"); break;
    case 7: Console.WriteLine("Июль"); break;
    case 8: Console.WriteLine("Август"); break;
    case 9: Console.WriteLine("Сентябрь"); break;
    case 10: Console.WriteLine("Октябрь"); break;
    case 11: Console.WriteLine("Ноябрь"); break;
    case 12: Console.WriteLine("Декабрь"); break;
    default: Console.WriteLine("Неверный номер"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 154. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program154
{
    internal class Program
    {
        static void Main(string[] args)
        {
        //Задача 54. Ввести номер месяца (1–12). Вывести количество дней в этом месяце (для невисокосного года).
int userInput273 = Convert.ToInt32(Console.ReadLine());
switch (userInput273)
{
    case 1: case 3: case 5: case 7: case 8: case 10: case 12:
        Console.WriteLine("31 день"); break;
    case 4: case 6: case 9: case 11:
        Console.WriteLine("30 дней"); break;
    case 2:
        Console.WriteLine("28 дней"); break;
    default: Console.WriteLine("Неверный номер"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 155. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program155
{
    internal class Program
    {
        static void Main(string[] args)
        {
         //Задача 55. Ввести номер месяца (1–12). Вывести название поры года («Зима», «Весна», «Лето», «Осень»).
int userInput274 = Convert.ToInt32(Console.ReadLine());
switch (userInput274)
{
    case 12: case 1: case 2: Console.WriteLine("Зима"); break;
    case 3: case 4: case 5: Console.WriteLine("Весна"); break;
    case 6: case 7: case 8: Console.WriteLine("Лето"); break;
    case 9: case 10: case 11: Console.WriteLine("Осень"); break;
    default: Console.WriteLine("Неверный номер"); break;
}
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>
---





> ### Программа 156. 
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program156
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 56. Ввести оценку студента (1–5). Вывести текстовое описание: 1 — «Очень плохо», 2 — «Неудовлетворительно», 3 — «Удовлетворительно», 4 — «Хорошо», 5 — «Отлично».
int userInput275 = Convert.ToInt32(Console.ReadLine());
switch (userInput275)
{
    case 1: Console.WriteLine("Очень плохо"); break;
    case 2: Console.WriteLine("Неудовлетворительно"); break;
    case 3: Console.WriteLine("Удовлетворительно"); break;
    case 4: Console.WriteLine("Хорошо"); break;
    case 5: Console.WriteLine("Отлично"); break;
    default: Console.WriteLine("Неверная оценка"); break;
}
        }
    }
}
        
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 157. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program157
{
    internal class Program
    {
        static void Main(string[] args)
        {
        //Задача 57. Реализовать простой калькулятор: ввести два вещественных числа и символ арифметической операции (+, -, *, /). Через switch выполнить вычисление. Предусмотреть защиту от деления на ноль.
double userInput276 = Convert.ToDouble(Console.ReadLine());
double userInput277 = Convert.ToDouble(Console.ReadLine());
char userInput278 = Convert.ToChar(Console.ReadLine());
switch (userInput278)
{
    case '+': Console.WriteLine(userInput276 + userInput277); break;
    case '-': Console.WriteLine(userInput276 - userInput277); break;
    case '*': Console.WriteLine(userInput276 * userInput277); break;
    case '/':
        if (userInput277 != 0) Console.WriteLine(userInput276 / userInput277);
        else Console.WriteLine("Деление на ноль!");
        break;
    default: Console.WriteLine("Неверная операция"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 158. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program158
{
    internal class Program
    {
        static void Main(string[] args)
        {
         //Задача 58. Ввести букву направления света (N, S, W, E). Вывести название направления («Север», «Юг», «Запад», «Восток»).
char userInput279 = Convert.ToChar(Console.ReadLine());
switch (userInput279)
{
    case 'N': Console.WriteLine("Север"); break;
    case 'S': Console.WriteLine("Юг"); break;
    case 'W': Console.WriteLine("Запад"); break;
    case 'E': Console.WriteLine("Восток"); break;
    default: Console.WriteLine("Неверное направление"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 159. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program159
{
    internal class Program
    {
        static void Main(string[] args)
        {
           //Задача 59. Ввести номер геометрической фигуры (1 — круг, 2 — прямоугольник, 3 — треугольник). Запросить соответствующие параметры фигуры и вычислить ее площадь.
int userInput280 = Convert.ToInt32(Console.ReadLine());
switch (userInput280)
{
    case 1:
        double userInput281 = Convert.ToDouble(Console.ReadLine());
        Console.WriteLine(Math.PI * userInput281 * userInput281);
        break;
    case 2:
        double userInput282 = Convert.ToDouble(Console.ReadLine());
        double userInput283 = Convert.ToDouble(Console.ReadLine());
        Console.WriteLine(userInput282 * userInput283);
        break;
    case 3:
        double userInput284 = Convert.ToDouble(Console.ReadLine());
        double userInput285 = Convert.ToDouble(Console.ReadLine());
        Console.WriteLine(0.5 * userInput284 * userInput285);
        break;
    default: Console.WriteLine("Неверная фигура"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 160. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program160
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 60. Ввести номер масти игральной карты (1 — пики, 2 — трефы, 3 — бубны, 4 — червы). Вывести название масти.
int userInput286 = Convert.ToInt32(Console.ReadLine());
switch (userInput286)
{
    case 1: Console.WriteLine("Пики"); break;
    case 2: Console.WriteLine("Трефы"); break;
    case 3: Console.WriteLine("Бубны"); break;
    case 4: Console.WriteLine("Червы"); break;
    default: Console.WriteLine("Неверная масть"); break;
}
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 161. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program161
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 61. Ввести достоинство карты (числа от 6 до 14). Вывести название: 11 — Валет, 12 — Дама, 13 — Король, 14 — Туз, остальные — по номиналу.
int userInput287 = Convert.ToInt32(Console.ReadLine());
switch (userInput287)
{
    case 11: Console.WriteLine("Валет"); break;
    case 12: Console.WriteLine("Дама"); break;
    case 13: Console.WriteLine("Король"); break;
    case 14: Console.WriteLine("Туз"); break;
    case 6: case 7: case 8: case 9: case 10:
        Console.WriteLine(userInput287); break;
    default: Console.WriteLine("Неверное достоинство"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>








> ### Программа 162. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program162
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 62. Ввести буквенное обозначение размера одежды (XS, S, M, L, XL, XXL). Вывести соответствующий российский размер (42, 44, 46, 48, 50, 52).
string userInput288 = Console.ReadLine();
switch (userInput288)
{
    case "XS": Console.WriteLine(42); break;
    case "S": Console.WriteLine(44); break;
    case "M": Console.WriteLine(46); break;
    case "L": Console.WriteLine(48); break;
    case "XL": Console.WriteLine(50); break;
    case "XXL": Console.WriteLine(52); break;
    default: Console.WriteLine("Неверный размер"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 163. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program163
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 63. Ввести номер единицы длины (1 — дециметр, 2 — километр, 3 — метр, 4 — миллиметр, 5 — сантиметр) и длину отрезка в этих единицах. Перевести и вывести длину в метрах.
int userInput289 = Convert.ToInt32(Console.ReadLine());
double userInput290 = Convert.ToDouble(Console.ReadLine());
switch (userInput289)
{
    case 1: Console.WriteLine(userInput290 / 10); break;
    case 2: Console.WriteLine(userInput290 * 1000); break;
    case 3: Console.WriteLine(userInput290); break;
    case 4: Console.WriteLine(userInput290 / 1000); break;
    case 5: Console.WriteLine(userInput290 / 100); break;
    default: Console.WriteLine("Неверная единица"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 164. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program164
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 64. Ввести номер единицы массы (1 — килограмм, 2 — миллиграмм, 3 — грамм, 4 — тонна, 5 — центнер) и массу. Вывести массу в килограммах.
int userInput291 = Convert.ToInt32(Console.ReadLine());
double userInput292 = Convert.ToDouble(Console.ReadLine());
switch (userInput291)
{
    case 1: Console.WriteLine(userInput292); break;
    case 2: Console.WriteLine(userInput292 / 1000000); break;
    case 3: Console.WriteLine(userInput292 / 1000); break;
    case 4: Console.WriteLine(userInput292 * 1000); break;
    case 5: Console.WriteLine(userInput292 * 100); break;
    default: Console.WriteLine("Неверная единица"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>







> ### Программа 165. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program165
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 65. Ввести код ошибки HTTP (200, 301, 400, 403, 404, 500, 502). Вывести текстовую расшифровку статуса.
int userInput293 = Convert.ToInt32(Console.ReadLine());
switch (userInput293)
{
    case 200: Console.WriteLine("OK"); break;
    case 301: Console.WriteLine("Moved Permanently"); break;
    case 400: Console.WriteLine("Bad Request"); break;
    case 403: Console.WriteLine("Forbidden"); break;
    case 404: Console.WriteLine("Not Found"); break;
    case 500: Console.WriteLine("Internal Server Error"); break;
    case 502: Console.WriteLine("Bad Gateway"); break;
    default: Console.WriteLine("Неизвестный код"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 166. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program166
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 66. Ввести код валюты (USD, EUR, CNY, RUB). Вывести полное наименование («Доллар США», «Евро», «Китайский юань», «Российский рубль»).
string userInput294 = Console.ReadLine();
switch (userInput294)
{
    case "USD": Console.WriteLine("Доллар США"); break;
    case "EUR": Console.WriteLine("Евро"); break;
    case "CNY": Console.WriteLine("Китайский юань"); break;
    case "RUB": Console.WriteLine("Российский рубль"); break;
    default: Console.WriteLine("Неизвестная валюта"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 167. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program167
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 67. Ввести символ клавиши управления движением персонажа (W, A, S, D в любом регистре). Вывести направление движения: вперед, влево, назад, вправо.
char userInput295 = Convert.ToChar(Console.ReadLine().ToUpper());
switch (userInput295)
{
    case 'W': Console.WriteLine("Вперед"); break;
    case 'A': Console.WriteLine("Влево"); break;
    case 'S': Console.WriteLine("Назад"); break;
    case 'D': Console.WriteLine("Вправо"); break;
    default: Console.WriteLine("Неверная клавиша"); break;
}


        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 168. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program168
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 68. Ввести номер цвета радуги (1–7). Вывести название цвета.
int userInput296 = Convert.ToInt32(Console.ReadLine());
switch (userInput296)
{
    case 1: Console.WriteLine("Красный"); break;
    case 2: Console.WriteLine("Оранжевый"); break;
    case 3: Console.WriteLine("Желтый"); break;
    case 4: Console.WriteLine("Зеленый"); break;
    case 5: Console.WriteLine("Голубой"); break;
    case 6: Console.WriteLine("Синий"); break;
    case 7: Console.WriteLine("Фиолетовый"); break;
    default: Console.WriteLine("Неверный номер"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 169. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program169
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 69. Ввести признак режима селектора АКПП (P, R, N, D, M). Вывести режим трансмиссии.
char userInput297 = Convert.ToChar(Console.ReadLine().ToUpper());
switch (userInput297)
{
    case 'P': Console.WriteLine("Парковка"); break;
    case 'R': Console.WriteLine("Задний ход"); break;
    case 'N': Console.WriteLine("Нейтраль"); break;
    case 'D': Console.WriteLine("Движение вперед"); break;
    case 'M': Console.WriteLine("Ручной режим"); break;
    default: Console.WriteLine("Неверный режим"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 170. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program170
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 70. Ввести номер пальца руки (1 — большой, 2 — указательный, 3 — средний, 4 — безымянный, 5 — мизинец). Вывести название пальца.
int userInput298 = Convert.ToInt32(Console.ReadLine());
switch (userInput298)
{
    case 1: Console.WriteLine("Большой"); break;
    case 2: Console.WriteLine("Указательный"); break;
    case 3: Console.WriteLine("Средний"); break;
    case 4: Console.WriteLine("Безымянный"); break;
    case 5: Console.WriteLine("Мизинец"); break;
    default: Console.WriteLine("Неверный номер"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>





> ### Программа 171. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program171
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 71. Ввести номер планеты от Солнца (1–8). Вывести название планеты Солнечной системы.
int userInput299 = Convert.ToInt32(Console.ReadLine());
switch (userInput299)
{
    case 1: Console.WriteLine("Меркурий"); break;
    case 2: Console.WriteLine("Венера"); break;
    case 3: Console.WriteLine("Земля"); break;
    case 4: Console.WriteLine("Марс"); break;
    case 5: Console.WriteLine("Юпитер"); break;
    case 6: Console.WriteLine("Сатурн"); break;
    case 7: Console.WriteLine("Уран"); break;
    case 8: Console.WriteLine("Нептун"); break;
    default: Console.WriteLine("Неверный номер"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 172. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program172
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 72. Ввести код тарифа мобильной связи (1 — Базовый, 2 — Студенческий, 3 — Безлимит). Вывести абонентскую плату и включенные гигабайты.
int userInput300 = Convert.ToInt32(Console.ReadLine());
switch (userInput300)
{
    case 1: Console.WriteLine("Базовый: 300 руб., 5 ГБ"); break;
    case 2: Console.WriteLine("Студенческий: 200 руб., 10 ГБ"); break;
    case 3: Console.WriteLine("Безлимит: 600 руб., без ограничений"); break;
    default: Console.WriteLine("Неверный тариф"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 173. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program173
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 73. Ввести номер квартала года (1–4). Вывести список входящих в него месяцев.
int userInput301 = Convert.ToInt32(Console.ReadLine());
switch (userInput301)
{
    case 1: Console.WriteLine("Январь, Февраль, Март"); break;
    case 2: Console.WriteLine("Апрель, Май, Июнь"); break;
    case 3: Console.WriteLine("Июль, Август, Сентябрь"); break;
    case 4: Console.WriteLine("Октябрь, Ноябрь, Декабрь"); break;
    default: Console.WriteLine("Неверный квартал"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 174. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program174
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 74. Ввести букву оценки американской системы (A, B, C, D, F). Вывести эквивалент в пятибалльной системе РФ.
char userInput302 = Convert.ToChar(Console.ReadLine().ToUpper());
switch (userInput302)
{
    case 'A': Console.WriteLine("5"); break;
    case 'B': Console.WriteLine("4"); break;
    case 'C': Console.WriteLine("3"); break;
    case 'D': Console.WriteLine("2"); break;
    case 'F': Console.WriteLine("1"); break;
    default: Console.WriteLine("Неверная оценка"); break;
}


        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 175. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program175
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 75. Ввести символ операции над множествами (U — объединение, I — пересечение, D — разность). Вывести расшифровку операции.
char userInput303 = Convert.ToChar(Console.ReadLine().ToUpper());
switch (userInput303)
{
    case 'U': Console.WriteLine("Объединение"); break;
    case 'I': Console.WriteLine("Пересечение"); break;
    case 'D': Console.WriteLine("Разность"); break;
    default: Console.WriteLine("Неверная операция"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 176. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program176
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 76. Ввести номер режима работы светофора (1 — Красный, 2 — Желтый, 3 — Зеленый, 4 — Мигающий желтый). Вывести предписание для водителя.
int userInput304 = Convert.ToInt32(Console.ReadLine());
switch (userInput304)
{
    case 1: Console.WriteLine("Стоп"); break;
    case 2: Console.WriteLine("Приготовиться"); break;
    case 3: Console.WriteLine("Ехать"); break;
    case 4: Console.WriteLine("Ехать с осторожностью"); break;
    default: Console.WriteLine("Неверный режим"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 177. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program177
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 77. Ввести цифру (0–9). Вывести ее словесное написание на русском языке.
int userInput305 = Convert.ToInt32(Console.ReadLine());
switch (userInput305)
{
    case 0: Console.WriteLine("Ноль"); break;
    case 1: Console.WriteLine("Один"); break;
    case 2: Console.WriteLine("Два"); break;
    case 3: Console.WriteLine("Три"); break;
    case 4: Console.WriteLine("Четыре"); break;
    case 5: Console.WriteLine("Пять"); break;
    case 6: Console.WriteLine("Шесть"); break;
    case 7: Console.WriteLine("Семь"); break;
    case 8: Console.WriteLine("Восемь"); break;
    case 9: Console.WriteLine("Девять"); break;
    default: Console.WriteLine("Не цифра"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 178. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program178
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 78. Ввести римскую цифру (I, V, X, L, C, D, M). Вывести ее арабское значение.
char userInput306 = Convert.ToChar(Console.ReadLine().ToUpper());
switch (userInput306)
{
    case 'I': Console.WriteLine(1); break;
    case 'V': Console.WriteLine(5); break;
    case 'X': Console.WriteLine(10); break;
    case 'L': Console.WriteLine(50); break;
    case 'C': Console.WriteLine(100); break;
    case 'D': Console.WriteLine(500); break;
    case 'M': Console.WriteLine(1000); break;
    default: Console.WriteLine("Неверная цифра"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 179. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program179
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 79. Ввести номер типа транспортного средства (1 — Мотоцикл, 2 — Легковой авто, 3 — Грузовой авто, 4 — Автобус). Вывести категорию водительского удостоверения (A, B, C, D).
int userInput307 = Convert.ToInt32(Console.ReadLine());
switch (userInput307)
{
    case 1: Console.WriteLine("A"); break;
    case 2: Console.WriteLine("B"); break;
    case 3: Console.WriteLine("C"); break;
    case 4: Console.WriteLine("D"); break;
    default: Console.WriteLine("Неверный тип"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 180. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program180
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 80. Ввести тип двигателя (1 — Бензиновый, 2 — Дизельный, 3 — Гибридный, 4 — Электрический). Вывести вид используемого источника энергии.
int userInput308 = Convert.ToInt32(Console.ReadLine());
switch (userInput308)
{
    case 1: Console.WriteLine("Бензин"); break;
    case 2: Console.WriteLine("Дизельное топливо"); break;
    case 3: Console.WriteLine("Бензин + электричество"); break;
    case 4: Console.WriteLine("Электричество"); break;
    default: Console.WriteLine("Неверный тип"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 181. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program181
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 81. Ввести номер операции в банкомате: 1 — Баланс, 2 — Снятие наличных, 3 — Пополнение, 4 — Перевод. Вывести сообщение о начале выбранной процедуры.
int userInput309 = Convert.ToInt32(Console.ReadLine());
switch (userInput309)
{
    case 1: Console.WriteLine("Проверка баланса..."); break;
    case 2: Console.WriteLine("Снятие наличных..."); break;
    case 3: Console.WriteLine("Пополнение счета..."); break;
    case 4: Console.WriteLine("Перевод средств..."); break;
    default: Console.WriteLine("Неверная операция"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 182. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program182
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 82. Ввести расширение файла (txt, cs, html, png, mp3). Вывести тип содержимого: текстовый документ, исходный код C#, веб-страница, изображение, аудиофайл.
string userInput310 = Console.ReadLine();
switch (userInput310)
{
    case "txt": Console.WriteLine("Текстовый документ"); break;
    case "cs": Console.WriteLine("Исходный код C#"); break;
    case "html": Console.WriteLine("Веб-страница"); break;
    case "png": Console.WriteLine("Изображение"); break;
    case "mp3": Console.WriteLine("Аудиофайл"); break;
    default: Console.WriteLine("Неизвестное расширение"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 183. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program183
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 83. Ввести номер химического элемента из первых пяти таблицы Менделеева (1–5). Вывести название элемента и его символ.
int userInput311 = Convert.ToInt32(Console.ReadLine());
switch (userInput311)
{
    case 1: Console.WriteLine("Водород (H)"); break;
    case 2: Console.WriteLine("Гелий (He)"); break;
    case 3: Console.WriteLine("Литий (Li)"); break;
    case 4: Console.WriteLine("Бериллий (Be)"); break;
    case 5: Console.WriteLine("Бор (B)"); break;
    default: Console.WriteLine("Неверный номер"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>









> ### Программа 184. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program184
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 84. Ввести код статуса заказа в интернет-магазине (NEW, PAID, SHIPPED, DELIVERED, CANCELED). Вывести подсказку для клиента.
string userInput312 = Console.ReadLine();
switch (userInput312)
{
    case "NEW": Console.WriteLine("Заказ создан, ожидает оплаты"); break;
    case "PAID": Console.WriteLine("Заказ оплачен, готовится к отправке"); break;
    case "SHIPPED": Console.WriteLine("Заказ отправлен"); break;
    case "DELIVERED": Console.WriteLine("Заказ доставлен"); break;
    case "CANCELED": Console.WriteLine("Заказ отменен"); break;
    default: Console.WriteLine("Неизвестный статус"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 185. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program185
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 85. Ввести код системы счисления (2, 8, 10, 16) и перевести введенное десятичное число в выбранную систему (через методы класса Convert).
int userInput313 = Convert.ToInt32(Console.ReadLine());
int userInput314 = Convert.ToInt32(Console.ReadLine());
switch (userInput313)
{
    case 2: Console.WriteLine(Convert.ToString(userInput314, 2)); break;
    case 8: Console.WriteLine(Convert.ToString(userInput314, 8)); break;
    case 10: Console.WriteLine(userInput314); break;
    case 16: Console.WriteLine(Convert.ToString(userInput314, 16)); break;
    default: Console.WriteLine("Неверная система счисления"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 186. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program186
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 86. Ввести номер курса колледжа (1–4). Вывести: «Первокурсник», «Второй курс», «Предвыпускной курс», «Выпускник».
int userInput315 = Convert.ToInt32(Console.ReadLine());
switch (userInput315)
{
    case 1: Console.WriteLine("Первокурсник"); break;
    case 2: Console.WriteLine("Второй курс"); break;
    case 3: Console.WriteLine("Предвыпускной курс"); break;
    case 4: Console.WriteLine("Выпускник"); break;
    default: Console.WriteLine("Неверный курс"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 187. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program187
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 87. Ввести код климатической зоны (1 — Арктическая, 2 — Субарктическая, 3 — Умеренная, 4 — Субтропическая, 5 — Тропическая). Вывести краткую характеристику.
int userInput316 = Convert.ToInt32(Console.ReadLine());
switch (userInput316)
{
    case 1: Console.WriteLine("Арктическая: очень холодно, полярная ночь"); break;
    case 2: Console.WriteLine("Субарктическая: холодная зима, короткое лето"); break;
    case 3: Console.WriteLine("Умеренная: четыре сезона"); break;
    case 4: Console.WriteLine("Субтропическая: тепло, мягкая зима"); break;
    case 5: Console.WriteLine("Тропическая: жарко и влажно"); break;
    default: Console.WriteLine("Неверный код"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 188. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program188
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 88. Ввести класс пожарной опасности (1–5). Вывести уровень угрозы и ограничения на посещение лесов.
int userInput317 = Convert.ToInt32(Console.ReadLine());
switch (userInput317)
{
    case 1: Console.WriteLine("Низкая опасность, посещение разрешено"); break;
    case 2: Console.WriteLine("Умеренная опасность, осторожно с огнем"); break;
    case 3: Console.WriteLine("Средняя опасность, ограничение костров"); break;
    case 4: Console.WriteLine("Высокая опасность, запрет на костры"); break;
    case 5: Console.WriteLine("Чрезвычайная опасность, посещение запрещено"); break;
    default: Console.WriteLine("Неверный класс"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 189. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program189
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 89. Ввести номер спортивного разряда (1 — Юношеский, 2 — Взрослый, 3 — КМС, 4 — МС, 5 — МСМК). Вывести расшифровку.
int userInput318 = Convert.ToInt32(Console.ReadLine());
switch (userInput318)
{
    case 1: Console.WriteLine("Юношеский разряд"); break;
    case 2: Console.WriteLine("Взрослый разряд"); break;
    case 3: Console.WriteLine("Кандидат в мастера спорта"); break;
    case 4: Console.WriteLine("Мастер спорта"); break;
    case 5: Console.WriteLine("Мастер спорта международного класса"); break;
    default: Console.WriteLine("Неверный разряд"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 190. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program190
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 90. Ввести код уровня доступа пользователя (G — Guest, U — User, M — Moderator, A — Administrator). Вывести перечень разрешенных действий.
char userInput319 = Convert.ToChar(Console.ReadLine().ToUpper());
switch (userInput319)
{
    case 'G': Console.WriteLine("Просмотр публичного контента"); break;
    case 'U': Console.WriteLine("Просмотр, комментарии"); break;
    case 'M': Console.WriteLine("Просмотр, комментарии, модерация"); break;
    case 'A': Console.WriteLine("Полный доступ"); break;
    default: Console.WriteLine("Неверный код"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 191. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program191
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 91. Ввести букву ноты (C, D, E, F, G, A, B). Вывести русское словесное обозначение (До, Ре, Ми, Фа, Соль, Ля, Си).
char userInput320 = Convert.ToChar(Console.ReadLine().ToUpper());
switch (userInput320)
{
    case 'C': Console.WriteLine("До"); break;
    case 'D': Console.WriteLine("Ре"); break;
    case 'E': Console.WriteLine("Ми"); break;
    case 'F': Console.WriteLine("Фа"); break;
    case 'G': Console.WriteLine("Соль"); break;
    case 'A': Console.WriteLine("Ля"); break;
    case 'B': Console.WriteLine("Си"); break;
    default: Console.WriteLine("Неверная нота"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 192. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program192
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 92. Ввести номер типа кузова автомобиля (1 — Седан, 2 — Хэтчбек, 3 — Универсал, 4 — Купе, 5 — Внедорожник). Вывести описание вместимости и компоновки.
int userInput321 = Convert.ToInt32(Console.ReadLine());
switch (userInput321)
{
    case 1: Console.WriteLine("Седан: 4-5 мест, отдельный багажник"); break;
    case 2: Console.WriteLine("Хэтчбек: 4-5 мест, укороченный кузов"); break;
    case 3: Console.WriteLine("Универсал: 5 мест, увеличенный багажник"); break;
    case 4: Console.WriteLine("Купе: 2-4 места, спортивный стиль"); break;
    case 5: Console.WriteLine("Внедорожник: 5-7 мест, повышенная проходимость"); break;
    default: Console.WriteLine("Неверный тип"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 193. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program193
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 93. Ввести код типа датчика охранной сигнализации: M (движение), D (открытие двери), S (дым), W (протечка воды). Вывести сообщение о типе угрозы.
char userInput322 = Convert.ToChar(Console.ReadLine().ToUpper());
switch (userInput322)
{
    case 'M': Console.WriteLine("Обнаружено движение"); break;
    case 'D': Console.WriteLine("Дверь открыта"); break;
    case 'S': Console.WriteLine("Обнаружен дым"); break;
    case 'W': Console.WriteLine("Протечка воды"); break;
    default: Console.WriteLine("Неизвестный датчик"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 194. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program194
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 94. Ввести номер фазы Луны (1 — Новолуние, 2 — Первая четверть, 3 — Полнолуние, 4 — Последняя четверть). Вывести характеристику фазы.
int userInput323 = Convert.ToInt32(Console.ReadLine());
switch (userInput323)
{
    case 1: Console.WriteLine("Новолуние: Луна не видна"); break;
    case 2: Console.WriteLine("Первая четверть: растущая Луна"); break;
    case 3: Console.WriteLine("Полнолуние: Луна полностью освещена"); break;
    case 4: Console.WriteLine("Последняя четверть: убывающая Луна"); break;
    default: Console.WriteLine("Неверный номер"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>


> ### Программа 195. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program195
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 95. Ввести символ разделителя пути в операционной системе (/ или \). Вывести, к какому семейству ОС относится разделитель (Unix/Linux или Windows).
char userInput324 = Convert.ToChar(Console.ReadLine());
switch (userInput324)
{
    case '/': Console.WriteLine("Unix/Linux"); break;
    case '\\': Console.WriteLine("Windows"); break;
    default: Console.WriteLine("Неверный символ"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>



> ### Программа 196. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program196
{
    internal class Program
    {
        static void Main(string[] args)
        {

//Задача 96. Ввести номер поколения мобильной связи (2, 3, 4, 5). Вывести название стандарта (GPRS/EDGE, UMTS/HSPA, LTE, NR) и типичную скорость.
int userInput325 = Convert.ToInt32(Console.ReadLine());
switch (userInput325)
{
    case 2: Console.WriteLine("GPRS/EDGE, до 0.3 Мбит/с"); break;
    case 3: Console.WriteLine("UMTS/HSPA, до 42 Мбит/с"); break;
    case 4: Console.WriteLine("LTE, до 1 Гбит/с"); break;
    case 5: Console.WriteLine("NR, до 20 Гбит/с"); break;
    default: Console.WriteLine("Неверное поколение"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>




> ### Программа 197. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program197
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 97. Ввести номер порта протокола (21, 22, 25, 80, 443). Вывести название сетевого протокола (FTP, SSH, SMTP, HTTP, HTTPS).
int userInput326 = Convert.ToInt32(Console.ReadLine());
switch (userInput326)
{
    case 21: Console.WriteLine("FTP"); break;
    case 22: Console.WriteLine("SSH"); break;
    case 25: Console.WriteLine("SMTP"); break;
    case 80: Console.WriteLine("HTTP"); break;
    case 443: Console.WriteLine("HTTPS"); break;
    default: Console.WriteLine("Неизвестный порт"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>

> ### Программа 198. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program198
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 98. Ввести код режима стиральной машины (1 — Хлопок, 2 — Синтетика, 3 — Шерсть, 4 — Быстрая 15 мин, 5 — Отжим). Вывести температуру стирки и скорость отжима.
int userInput327 = Convert.ToInt32(Console.ReadLine());
switch (userInput327)
{
    case 1: Console.WriteLine("Хлопок: 60°C, 1200 об/мин"); break;
    case 2: Console.WriteLine("Синтетика: 40°C, 800 об/мин"); break;
    case 3: Console.WriteLine("Шерсть: 30°C, 600 об/мин"); break;
    case 4: Console.WriteLine("Быстрая 15 мин: 30°C, 800 об/мин"); break;
    case 5: Console.WriteLine("Отжим: без стирки, 1400 об/мин"); break;
    default: Console.WriteLine("Неверный режим"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 199. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program199
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 99. Ввести код тарифной зоны электроэнергии (1 — Пик, 2 — Полупик, 3 — Ночь). Вывести стоимость киловатт-часа.
int userInput328 = Convert.ToInt32(Console.ReadLine());
switch (userInput328)
{
    case 1: Console.WriteLine("Пик: 7 руб./кВт·ч"); break;
    case 2: Console.WriteLine("Полупик: 5 руб./кВт·ч"); break;
    case 3: Console.WriteLine("Ночь: 3 руб./кВт·ч"); break;
    default: Console.WriteLine("Неверная зона"); break;
}
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>






> ### Программа 200. 

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Program200
{
    internal class Program
    {
        static void Main(string[] args)
        {
//Задача 100. Ввести код состояния потока выполнения в C# (Running, Suspended, Stopped, Aborted). Вывести пояснение жизненного цикла потока.
string userInput329 = Console.ReadLine();
switch (userInput329)
{
    case "Running": Console.WriteLine("Поток выполняется"); break;
    case "Suspended": Console.WriteLine("Поток приостановлен"); break;
    case "Stopped": Console.WriteLine("Поток завершен"); break;
    case "Aborted": Console.WriteLine("Поток прерван"); break;
    default: Console.WriteLine("Неизвестное состояние"); break;
}

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="">
</picture>
```
🧑‍💻 Ссылка на практическую работу №1 и преподавателя [github](https://github.com/U5er01Task/Fundamentals-of-Algorithmization-and-Programming-2026/tree/main) - [Преподаватель](https://github.com/U5er01Task)

---
