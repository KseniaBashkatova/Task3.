># Практическая работа №1: Базовые типы данных, консольный ввод-вывод и приведение типов в C#



> ### Программа 1. Вывод ФИО в одну строку



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
            // Напишите программу, которая запрашивает у пользователя фамилию, имя и отчество по отдельности, а затем выводит их одной строкой в формате: Фамилия И. О..
            Console.Write("Введите фамилию: ");
            string lastName = Console.ReadLine();
            Console.Write("Введите имя: ");
            string firstName = Console.ReadLine();
            Console.Write("Введите отчество: ");
            string middleName = Console.ReadLine();
            Console.WriteLine($"{lastName} {firstName[0]}. {middleName[0]}.");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program1.jpg">
</picture>


> ### Программа 2. Арифметические вычисления, остаток от деления.

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
            //Запросите у пользователя два целых числа. Выведите их сумму, разность, произведение, а также целочисленное частное и остаток от деления.
            Console.Write("Введите первое целое число: ");
            int a = int.Parse(Console.ReadLine());
            Console.Write("Введите второе целое число: ");
            int b = int.Parse(Console.ReadLine());
            Console.WriteLine($"Сумма: {a + b}");
            Console.WriteLine($"Разность: {a - b}");
            Console.WriteLine($"Произведение: {a * b}");
            Console.WriteLine($"Целочисленное частное: {a / b}");
            Console.WriteLine($"Остаток от деления: {a % b}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program2.png">
</picture>
> ### Программа 3. Перевод температуры из градусах Цельсия в градусы Фаренгейта

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
            //Пользователь вводит температуру в градусах Цельсия. Переведите ее в градусы Фаренгейта по формуле: F = C × 9/5 +32
            Console.Write("Введите температуру в градусах Цельсия: ");
            double c = double.Parse(Console.ReadLine());
            double f = c * 9.0 / 5.0 + 32.0;
            Console.WriteLine($"Температура по Фаренгейту: {f:F2}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program3.png">
</picture>




> ### Программа 4. Рассчет объема куба и площадь его полной поверхности.

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
         //Запросите длину ребра куба. Рассчитайте объем куба и площадь его полной поверхности.
         Console.Write("Введите длину ребра куба: ");
         double a = double.Parse(Console.ReadLine());
         double volume = a * a * a;
         double surfaceArea = 6 * a;
         Console.WriteLine($"Объём куба: {volume:F2}");
         Console.WriteLine($"Площадь полной поверхности: {surfaceArea:F2}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program4.png">
</picture>



> ### Программа 5. Перевод значения в часы, минуты и секунды

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
         // Запросите у пользователя количество секунд. Переведите это значение в часы, минуты и секунды (например, 3665 сек -> 1 ч, 1 мин, 5 сек).
            Console.Write("Введите количество секунд: ");
         int totalSeconds = int.Parse(Console.ReadLine());
         int hours = totalSeconds / 3600;
         int minutes = (totalSeconds % 3600) / 60;
         int seconds = totalSeconds % 60;
         Console.WriteLine($"{hours} ч, {minutes} мин, {seconds} сек");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program5.png">
</picture>
---

> ### Программа 6. Расчет двух целочисленных переменных

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
         //Реализуйте обмен значениями двух целочисленных переменных a и b, введенных с клавиатуры, сначала с использованием третьей переменной, затем без нее (арифметическим способом).
         Console.Write("Введите а: ");
         int a = int.Parse(Console.ReadLine());
         Console.Write("Введите b: ");
         int b = int.Parse(Console.ReadLine());
         int originalA = a;
         int originalB = b;
         Console.WriteLine($"Исходные значения: a = {a}, b = {b}");
         // Обмен с использованием третьей переменной
         int temp = a;
         a = b;
         b = temp;
         Console.WriteLine($"После обмена с третьей переменной: a = {a}, b = {b}");
         // Возвращаем исходные значения
         a = originalA;
         b = originalB;
         // Обмен без третьей переменной, арифметическим способом
         a = a + b;
         b = a - b;
         a = a - b;
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program6.png">
</picture>
> ### Программа 7. Расчет среднего арифметического

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
         //Запросите три вещественных числа. Вычислите и выведите их среднее арифметическое с округлением до двух знаков после запятой.
         Console.Write("Введите первое число: ");
         double a = double.Parse(Console.ReadLine());
         Console.Write("Введите второе число: ");
         double b = double.Parse(Console.ReadLine());
         Console.Write("Введите третье число: ");
         double c = double.Parse(Console.ReadLine());
         double average = (a + b + c) / 3.0;
         Console.WriteLine($"Среднее арифметическое: {average:F2}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program7.png">
</picture>
> ### Программа 8. Расчет скорости движения

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
         //Считайте расстояние в метрах и время в секундах. Рассчитайте и выведите скорость движения в км/ч.
         Console.Write("Введите расстояние в метрах: ");
         double meters = double.Parse(Console.ReadLine());

         Console.Write("Введите время в секундах: ");
         double seconds = double.Parse(Console.ReadLine());

         double speedKmH = (meters / 1000) / (seconds / 3600);
         Console.WriteLine($"Скорость: {speedKmH:F2} км/ч");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program8.png">
</picture>
> ### Программа 9. Расчет скидки

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
            //Запросите стоимость товара и процент скидки (от 0 до 100). Вычислите сумму скидки и итоговую цену товара с использованием типа decimal.
            Console.Write("Введите стоимость товара: ");
            decimal price = decimal.Parse(Console.ReadLine());
            Console.Write("Введите процент скидки от 0 до 100: ");
            decimal discountPercent = decimal.Parse(Console.ReadLine());
            decimal discountAmount = price * discountPercent / 100m;
            decimal finalPrice = price - discountAmount;
            Console.WriteLine($"Сумма скидки: {discountAmount:F2}");
            Console.WriteLine($"Итоговая цена: {finalPrice:F2}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program9.png">
</picture>
> ### Программа 10. Расчет стоимости разговора

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
            //Пользователь вводит баланс мобильного телефона и стоимость одной минуты разговора. Вычислите, сколько полных минут разговора доступно абоненту.
            Console.Write("Введите баланс мобильного телефона: ");
            decimal balance = decimal.Parse(Console.ReadLine());
            Console.Write("Введите стоимость одной минуты разговора: ");
            decimal costPerMinute = decimal.Parse(Console.ReadLine());
            int fullMinutes = (int)Math.Floor(balance / costPerMinute);
            Console.WriteLine($"Доступно полных минут разговора: {fullMinutes}");
        }
    }
}
```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program10.png">
</picture>
```
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
//Напишите программу, которая с помощью оператора sizeof определяет и выводит размеры в байтах для типов: sbyte, short, int, long, float, double, decimal, char, bool.
         Console.WriteLine("Размеры типов данных в байтах:\n");
         Console.WriteLine($"sbyte: {sizeof(sbyte)} байт");
         Console.WriteLine($"short: {sizeof(short)} байт");
         Console.WriteLine($"int: {sizeof(int)} байт");
         Console.WriteLine($"long: {sizeof(long)} байт");
         Console.WriteLine($"float: {sizeof(float)} байт");
         Console.WriteLine($"double: {sizeof(double)} байт");
         Console.WriteLine($"decimal: {sizeof(decimal)} байт");
         Console.WriteLine($"char: {sizeof(char)} байт");
         Console.WriteLine($"bool: {sizeof(bool)} байт");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program11.png">
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
 //Выведите на консоль минимальные и максимальные значения всех целочисленных типов, используя поля MinValue и MaxValue.
         Console.WriteLine($"sbyte:   Min = {sbyte.MinValue}, Max = {sbyte.MaxValue}");
         Console.WriteLine($"short:   Min = {short.MinValue:N0}, Max = {short.MaxValue:N0}");
         Console.WriteLine($"int:     Min = {int.MinValue:N0}, Max = {int.MaxValue:N0}");
         Console.WriteLine($"long:    Min = {long.MinValue:N0}, Max = {long.MaxValue:N0}");
         Console.WriteLine($"byte:    Min = {byte.MinValue}, Max = {byte.MaxValue}");
         Console.WriteLine($"ushort:  Min = {ushort.MinValue:N0}, Max = {ushort.MaxValue:N0}");
         Console.WriteLine($"uint:    Min = {uint.MinValue:N0}, Max = {uint.MaxValue:N0}");
         Console.WriteLine($"ulong:   Min = {ulong.MinValue:N0}, Max = {ulong.MaxValue:N0}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program12.png">
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
// Продемонстрируйте эффект циклического переполнения (overflow): увеличьте значение переменной типа byte, равное 255, на 1 внутри блока unchecked и внутри блока checked.
byte value = 255;

// unchecked: переполнение "зацикливается" — 255 + 1 = 0
byte uncheckedResult = unchecked((byte)(value + 1));
Console.WriteLine($"unchecked: 255 + 1 = {uncheckedResult}");

// checked: переполнение вызывает OverflowException,


// Вариант 1: демонстрация через checked-выражение,
// которое выбросит исключение и завершит программу.
Console.WriteLine("checked: попытка вычислить 255 + 1...");
byte checkedResult = checked((byte)(value + 1));
Console.WriteLine($"checked: {checkedResult}"); // сюда не дойдём
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program13.png">
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
 // Считайте с клавиатуры строку, содержащую один символ. Определите код этого символа в кодировке Unicode и следующий за ним символ в таблице.
 Console.Write("Введите один символ: ");
 ConsoleKeyInfo keyInfo = Console.ReadKey();
 char inputChar = keyInfo.KeyChar;

 Console.WriteLine();
 // Получение кода Unicode через явное приведение к целому числу
 int codePoint = (int)inputChar;
 // следующий символ по таблице.
 // приведение обратно к типу char обязательно
 char nextChar = (char)(codePoint + 1);
 Console.WriteLine($"Символ: {inputChar}");
 Console.WriteLine($"Код Unicode (десятичный): {codePoint}");
 Console.WriteLine($"Код Unicode (шестнадцатеричный): U+{codePoint:X4}");
 Console.WriteLine($"Следующий символ: {nextChar} (код {(codePoint + 1)})");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program14.png">
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
 // Напишите программу, запрашивающую логическое значение (true/false) с клавиатуры с помощью bool.Parse и инвертирующую его.
        Console.Write("Выберите логическое значение (true/false): ");
        bool value = bool.Parse(Console.ReadLine());

        bool inverted = !value;

        Console.WriteLine($"Введено: {value}");
        Console.WriteLine($"Инвертировано: {inverted}");
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program15.png">
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
 // Сделайте программу, которая запрашивает число с плавающей точкой и выводит отдельно его целую и дробную части.

            Console.Write("Введите число с плавающей точкой: ");
            double number = Convert.ToDouble(Console.ReadLine());

            double integerPart = Math.Truncate(number);
            double fractionalPart = number - integerPart;

            Console.WriteLine("Целая часть:   " + integerPart);
            Console.WriteLine("Дробная часть: " + fractionalPart);

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program16.png">
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
 // Создайте переменные типов float и double, присвойте им значение  1.0/3.0 и выведите на экран с максимальным количеством знаков, чтобы показать разницу в точности.  
            float floatValue = 1.0f / 3.0f;
            double doubleValue = 1.0 / 3.0;

            // "G9" для float — 9 значащих цифр (максимум для float)
            // "G17" для double — 17 значащих цифр (максимум для double)
            Console.WriteLine("float  (G9):  " + floatValue.ToString("G9"));
            Console.WriteLine("double (G17): " + doubleValue.ToString("G17"));

            // Для наглядности — с фиксированным числом знаков после запятой
            Console.WriteLine();
            Console.WriteLine("float  (F20): " + floatValue.ToString("F20"));
            Console.WriteLine("double (F20): " + doubleValue.ToString("F20"));

            // Разница
            Console.WriteLine();
            Console.WriteLine("Разница: " + ((double)floatValue - doubleValue).ToString("G17"));

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program17.png">
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
       // Напишите программу, которая вычисляет разницу между операциями сложения над double и над decimal (сложите 0.1 десять раз и сравните результат с 1.0).
            double d = 0.0;
            decimal m = 0.0m;

            for (int i = 0; i < 10; i++)
            {
                d = d + 0.1;
                m = m + 0.1m;
            }

            Console.WriteLine("double:  " + d);
            Console.WriteLine("decimal: " + m);
            Console.WriteLine("double == 1.0:  " + (d == 1.0));
            Console.WriteLine("decimal == 1.0: " + (m == 1.0m));
        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program18.png">
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
// Считайте число типа long и выясните, поместится ли оно в диапазон типа short без переполнения.
            Console.Write("Введите число: ");
            long x = long.Parse(Console.ReadLine());

            Console.WriteLine("Поместится в short: " + (x >= -32768 && x <= 32767));

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program19.png">
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
   // Запросите у пользователя символ цифровой клавиши (от '0' до '9') и преобразуйте его в соответствующее целочисленное значение (int) без использования строк. 
            Console.Write("Введите цифру от 0 до 9: ");
            char c = Console.ReadKey().KeyChar;
            Console.WriteLine();

            int x = c - '0';

            Console.WriteLine("Число: " + x);

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program20.png">
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
 // Объявите константу гравитационного ускорения g = 9.80665. Запросите массу тела и высоту. Вычислите потенциальную энергию тела:  E =m⋅g⋅h. 
            // это константа гравитационного ускорения
            const double g = 9.80665;

            // Запрашиваем массу тела
            Console.Write("Введите массу тела (кг): ");
            double m = double.Parse(Console.ReadLine());

            // Запрашиваем высоту
            Console.Write("Введите высоту (м): ");
            double h = double.Parse(Console.ReadLine());

            // Вычисляем потенциальную энергию
            double E = m * g * h;

            // Выводим результат
            Console.WriteLine($"Потенциальная энергия тела: {E:F2} Дж");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program21.png">
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
  // Объявите константу числа  π. Рассчитайте объем и площадь поверхности сферы по заданному радиусу.
            // константа числа пи 
            const double Pi = 3.14159265358979;

            // Запрашиваем радиус сферы
            Console.Write("Введите радиус сферы (м): ");
            double r = double.Parse(Console.ReadLine());

            // Вычисляем объём сферы: V = (4/3) * π * r³
            double V = (4.0 / 3.0) * Pi * r * r * r;

            // Вычисляем площадь поверхности сферы: S = 4 * π * r²
            double S = 4 * Pi * r * r;

            // Выводим результаты
            Console.WriteLine($"Объём сферы:              {V:F2} м³");
            Console.WriteLine($"Площадь поверхности сферы: {S:F2} м²");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program22.png">
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
  // С помощью констант дней недели (1 — Понедельник, 7 — Воскресенье) и введенного номера дня выведите название дня недели.
            // Объявляем константы дней недели
            const int Monday = 1;
            const int Tuesday = 2;
            const int Wednesday = 3;
            const int Thursday = 4;
            const int Friday = 5;
            const int Saturday = 6;
            const int Sunday = 7;

            // Запрашиваем номер дня недели
            Console.Write("Введите номер дня недели (1–7): ");
            int day = Convert.ToInt32(Console.ReadLine());

            // Определяем название дня 
            if (day == Monday)
            {
                Console.WriteLine("Понедельник");
            }
            else if (day == Tuesday)
            {
                Console.WriteLine("Вторник");
            }
            else if (day == Wednesday)
            {
                Console.WriteLine("Среда");
            }
            else if (day == Thursday)
            {
                Console.WriteLine("Четверг");
            }
            else if (day == Friday)
            {
                Console.WriteLine("Пятница");
            }
            else if (day == Saturday)
            {
                Console.WriteLine("Суббота");
            }
            else if (day == Sunday)
            {
                Console.WriteLine("Воскресенье");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program23.png">
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
 // Запросите координаты двух точек на плоскости (x1,y1) и (x2,y2).Вычислите расстояние между ними по евклидовой метрике.
            Console.Write("Введи x1: ");
            double x1 = double.Parse(Console.ReadLine());

            Console.Write("Введи y1: ");
            double y1 = double.Parse(Console.ReadLine());

            Console.Write("Введи x2: ");
            double x2 = double.Parse(Console.ReadLine());

            Console.Write("Введи y2: ");
            double y2 = double.Parse(Console.ReadLine());

            double dx = x2 - x1; 
            double dy = y2 - y1;

            // Квадрат расстояния: (x2−x1)² + (y2−y1)²
            double square = dx * dx + dy * dy;

            // Расстояние = √square
            double distance = Math.Sqrt(square);

            Console.WriteLine($"Расстояние: {distance:F2}");

        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program24.png">
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
 // Объявите константу базовой процентной ставки банка. Запросите сумму вклада и срок в месяцах. Рассчитайте сумму простых процентов: I = P × r × t / 12

            // базовая процентная ставка банка 
            const double r = 0.14;

            Console.Write("Введи сумму вклада (руб): ");
            double P = double.Parse(Console.ReadLine());

            Console.Write("Введи срок вклада (в месяцах): ");
            double t = double.Parse(Console.ReadLine());

            // вычисляем простые проценты: I = P × r × t / 12
            double I = P * r * t / 12;

            // выводим результат
            Console.WriteLine($"Сумма простых процентов: {I:F2} руб.");


        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program25.png">
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
// Запросите катеты прямоугольного треугольника. Вычислите гипотенузу и радиус вписанной окружности: r = (a + b - c) / 2

            // Запрашиваем катеты
            Console.Write("Введи катет a: ");
            double a = double.Parse(Console.ReadLine());

            Console.Write("Введи катет b: ");
            double b = double.Parse(Console.ReadLine());

            // Вычисляем гипотенузу по теореме Пифагора: c = √(a² + b²)
            double c = Math.Sqrt(a * a + b * b);

            // Вычисляем радиус вписанной окружности: r = (a + b − c) / 2
            double r = (a + b - c) / 2;

            // Выводим результаты
            Console.WriteLine($"Гипотенуза: {c:F2}");
            Console.WriteLine($"Радиус вписанной окружности: {r:F2}");

        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program26.png">
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
  // Задайте константу скорости света c =  299792458 м / с.Запросите массу в килограммах и рассчитайте эквивалентную энергию по формуле E=m⋅c2 
            // Константа скорости света (м/с)
            const long c = 299792458;

            // Запрашиваем массу в килограммах
            Console.Write("Введи массу тела (кг): ");
            double m = double.Parse(Console.ReadLine());

            // Вычисляем энергию по формуле E = m · c²
            double E = m * (double)c * c;

            // Выводим результат
            Console.WriteLine($"Эквивалентная энергия: {E:E3} Дж");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program27.png">
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
  // Рассчитайте индекс массы тела (ИМТ) по формуле: BMI=вес / рост2, где вес задан в кг, а рост — в метрах.
            Console.Write("Введите вес (кг): ");
            double weight = double.Parse(Console.ReadLine());

            Console.Write("Введи рост (м): ");
            double height = double.Parse(Console.ReadLine());

            // Вычисляем ИМТ: вес / рост²
            double bmi = weight / (height * height);

            Console.WriteLine($"Индекс массы тела: {bmi:F2}");

        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program28.png">
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
// Объявите константы перевода единиц: дюймы в сантиметры, футы в метры, фунты в килограммы. Считайте значения в англо-американской системе и выведите в метрической.
            // Константы перевода единиц
            const double InchToCm = 2.54;      
            const double FootToM = 0.3048;   
            const double PoundToKg = 0.453592;  

            // Запрашиваем значения в англо-американской системе
            Console.Write("Введи рост в футах: ");
            double feet = double.Parse(Console.ReadLine());

            Console.Write("Введи рост в дюймах: ");
            double inches = double.Parse(Console.ReadLine());

            Console.Write("Введи вес в фунтах: ");
            double pounds = double.Parse(Console.ReadLine());

            // Переводим в метрическую систему
            double heightM = feet * FootToM + inches * InchToCm / 100;
            double weightKg = pounds * PoundToKg;

            // Выводим результаты
            Console.WriteLine($"Рост: {heightM:F2} м");
            Console.WriteLine($"Вес:  {weightKg:F2} кг");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program29.png">
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
// Запросите коэффициент сопротивления и силу тока. Используя закон Ома и константу времени, рассчитайте выделившееся количество теплоты по закону Джоуля-Ленца
            Console.Write("Введите сопротивление R (Ом): ");
            double R = double.Parse(Console.ReadLine());

            Console.Write("Введите силу тока I (А): ");
            double I = double.Parse(Console.ReadLine());

            // Константа времени t (в секундах) — можно задать или запросить
            Console.Write("Введите время t (с): ");
            double t = double.Parse(Console.ReadLine());

            // По закону Джоуля-Ленца: Q = I^2 * R * t
            double Q = I * I * R * t;

            Console.WriteLine($"Выделившееся количество теплоты Q = {Q:F2} Дж");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program30.png">
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
// Пользователь вводит дробное число типа double. Преобразуйте его в int путем явного отбрасывания дробной части и путем округления до ближайшего целого через Math.Round. Сравните результаты.
            Console.Write("Введите дробное число: ");
            double number = double.Parse(Console.ReadLine());

            // Приведение к int
            int truncated = (int)number;

            // Округление до ближайшего целого 
            int rounded = (int)Math.Round(number);

            // Вывод результатов
            Console.WriteLine($"Исходное число:        {number}");
            Console.WriteLine($"Отбрасывание дробной:  {truncated}");
            Console.WriteLine($"Округление Math.Round: {rounded}");

            // Сравнение
            if (truncated == rounded)
                Console.WriteLine("Результаты совпадают.");
            else
                Console.WriteLine($"Результаты различаются на {Math.Abs(rounded - truncated)}.");

        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program31.png">
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
 // Запросите строку с клавиатуры. Используя метод int.TryParse, выведите результат проверки: успешно ли число преобразовано или произошла ошибка ввода.

            Console.Write("Введите строку: ");
            string input = Console.ReadLine();

            // Пытаемся преобразовать строку в int через TryParse
            bool success = int.TryParse(input, out int number);

            // Выводим результат проверки
            if (success)
            {
                Console.WriteLine($"Преобразование успешно. Число: {number}");
            }
            else
            {
                Console.WriteLine("Ошибка ввода: строку не удалось преобразовать в целое число.");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program32.png">
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
// Преобразуйте символьную переменную char, содержащую букву, в тип int, прибавьте 32 (переход между регистрами в ASCII для латиницы) и преобразуйте обратно в char.
            // Символьная переменная, содержащая заглавную латинскую букву
            Console.Write("Введите заглавную латинскую букву: ");
            char letter = char.Parse(Console.ReadLine());

            // Преобразуем char в int (получаем ASCII-код)
            int code = (int)letter;

            // Прибавляем 32 — переход от заглавной к строчной в ASCII
            int newCode = code + 32;

            // Преобразуем обратно в char
            char lowerLetter = (char)newCode;

            // Вывод результатов
            Console.WriteLine($"Исходная буква: '{letter}' (код {code})");
            Console.WriteLine($"После +32: код {newCode}");
            Console.WriteLine($"Результат: '{lowerLetter}'");

        }
    }
}

```


`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program33.png">
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
// Считайте число типа double. Выполните его приведение последовательно к float, long, int, short и byte. Выведите значение на каждом шаге.
            Console.Write("Введите число типа double: ");
            double value = double.Parse(Console.ReadLine());

            Console.WriteLine($"Исходное значение (double): {value}");

            // double -> float
            float f = (float)value;
            Console.WriteLine($"После приведения к float: {f}");

            // float -> long
            long l = (long)f;
            Console.WriteLine($"После приведения к long: {l}");

            // long -> int
            int i = (int)l;
            Console.WriteLine($"После приведения к int: {i}");

            // int -> short
            short s = (short)i;
            Console.WriteLine($"После приведения к short: {s}");

            // short -> byte
            byte b = (byte)s;
            Console.WriteLine($"После приведения к byte: {b}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program34.png">
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
// Пользователь вводит три строковых значения. Попробуйте распарсить первое в int, второе в double, третье в bool. Выведите статус конвертации каждого значения.
            // Запрашиваем три строковых значения
            Console.Write("Введите значение для int: ");
            string s1 = Console.ReadLine();

            Console.Write("Введите значение для double: ");
            string s2 = Console.ReadLine();

            Console.Write("Введите значение для bool: ");
            string s3 = Console.ReadLine();

            Console.WriteLine("<> Результаты конвертации <>");

            // Использование тернального оператора для парсинга значений
            Console.WriteLine(int.TryParse(s1, out int iv)
                       ? $"[int] Успех: {s1} -> {iv}"
                       : $"[int] Ошибка: {s1} не является целым числом");

            Console.WriteLine(double.TryParse(s2, out double dv)
                ? $"[double] Успех: {s2} -> {dv}"
                : $"[double] Ошибка: {s2} не является числом с плавающей точкой");

            Console.WriteLine(bool.TryParse(s3, out bool bv)
                ? $"[bool] Успех: {s3} > {bv}"
                : $"[bool] Ошибка: {s3} не является логическим значением");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program35.png">
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
  // Напишите программу, которая принимает целое четырехзначное число и раскладывает его на отдельные цифры с помощью математических операций деления и остатка, преобразуя каждую цифру в byte.
            // Запрашиваем четырёхзначное целое число
            Console.Write("Введите четырёхзначное число: ");
            int number = int.Parse(Console.ReadLine());

            // Раскладываем на цифры с помощью деления и остатка
            byte thousands = (byte)(number / 1000);            // тысячи
            byte hundreds = (byte)((number / 100) % 10);      // сотни
            byte tens = (byte)((number / 10) % 10);       // десятки
            byte units = (byte)(number % 10);              // единицы

            // Вывод результата
            Console.WriteLine($"Число {number} состоит из цифр:");
            Console.WriteLine($"Тысячи:   {thousands}");
            Console.WriteLine($"Сотни:    {hundreds}");
            Console.WriteLine($"Десятки:  {tens}");
            Console.WriteLine($"Единицы:  {units}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program36.png">
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
// Создайте переменную типа object, поместите туда значение int (упаковка/boxing), затем извлеките его обратно в int (распаковка/unboxing), а также продемонстрируйте ошибку InvalidCastException при попытке распаковать в short.
            // Упаковка
            Console.Write("Введите значение типа int: ");
            int zapros = int.Parse(Console.ReadLine());

            object boxed = (object)zapros;
            Console.WriteLine($"boxed = {boxed}");

            // Распаковка в int
            int unboxed = (int)boxed;
            Console.WriteLine($"unboxed = {unboxed}");

            // Попытка распаковать в short
            try
            {
                short wrong = (short)boxed;
                Console.WriteLine(wrong);
            }
            catch (InvalidCastException ex)
            {
                Console.WriteLine($"InvalidCastException: {ex.Message}");
            }

            // Корректно: сначала в int, потом в short
            short correct = (short)(int)boxed;
            Console.WriteLine($"correct = {correct}");

        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program37.png">
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
//Запросите у пользователя шестнадцатеричную строку (например, "FF" или "1A") и преобразуйте ее в десятичное целое число с помощью Convert.ToInt32(input, 16).

        Console.Clear();

        Console.ForegroundColor = ConsoleColor.DarkGreen;
        Console.WriteLine("Преобразование шестнадцатеричной строки в десятичное число");
        Console.ForegroundColor = ConsoleColor.Gray;

        Console.WriteLine("Введите шестнадцатеричное число (например, FF или 1A): ");
        string input = Console.ReadLine();

        int result = Convert.ToInt32(input, 16);

        Console.WriteLine($"Шестнадцатеричное: {input}");
        Console.WriteLine($"Десятичное:       {result}");

        }
    }
}

```

`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program38.png">
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
// Продемонстрируйте сужающее преобразование с потерей старших битов: запишите число 300 в переменную типа int и явно приведите ее к byte. Объясните полученный результат.

            // Задаём число 300 в переменную типа int
            int number = 300;

            // Явное сужающее приведение int -> byte
            byte result = (byte)number;

            // Вывод результата
            Console.WriteLine($"Исходное значение (int):  {number}");
            Console.WriteLine($"После приведения (byte):  {result}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program39.png">
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
 // Пользователь вводит значение типа float. Проверьте, является ли введенное значение бесконечностью (float.IsInfinity) или неопределенностью (float.IsNaN).
            // Запрашиваем значение
            Console.Write("Введите значение (число, Infinity, -Infinity или NaN): ");
            string input = Console.ReadLine();

            // Весь код — через тернарный оператор
            Console.WriteLine(
                !float.TryParse(input, System.Globalization.NumberStyles.Float,
                System.Globalization.CultureInfo.InvariantCulture, out float value)
                ? $"Ошибка: {input} не является числом float."
                : float.IsInfinity(value)
                ? $"{value} — бесконечность"
                : float.IsNaN(value)
                ? $"{value} — неопределённость (NaN)"
                : $"{value} — обычное число");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program40.png">
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
 // Расчет чека в ресторане: Подсчитайте стоимость блюд (тип decimal), размер сервисного сбора в процентах и количество персон. Рассчитайте общую сумму к оплате и сумму на каждого гостя.

            Console.Clear();
            Console.ForegroundColor = ConsoleColor.DarkGreen;
            Console.WriteLine("Расчёт чека в ресторане");
            Console.ForegroundColor = ConsoleColor.Gray;

            Console.WriteLine("Введите стоимость блюд: ");
            decimal name1 = Convert.ToDecimal(Console.ReadLine());

            Console.WriteLine("Введите размер сервисного сбора (%): ");
            decimal name2 = Convert.ToDecimal(Console.ReadLine());

            Console.WriteLine("Введите количество персон: ");
            int name3 = Convert.ToInt32(Console.ReadLine());

            decimal name4 = name1 * name2 / 100;
            decimal name5 = name1 + name4;
            decimal name6 = name5 / name3;

            Console.WriteLine($"Стоимость блюд: {name1:F2}");
            Console.WriteLine($"Сервисный сбор ({name2}%): {name4:F2}");
            Console.WriteLine($"Итого к оплате: {name5:F2}");
            Console.WriteLine($"На каждого гостя: {name6:F2}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program41.png">
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
 // Расход топлива: Запросите пройденное расстояние в километрах, средний расход топлива на 100 км и текущую стоимость литра бензина. Вычислите необходимое количество литража и итоговые финансовые затраты на поездку.

           Console.Clear();

Console.ForegroundColor = ConsoleColor.DarkGreen;
Console.WriteLine("Расчёт затрат на топливо");
Console.ForegroundColor = ConsoleColor.Gray;

Console.WriteLine("Введите пройденное расстояние (км): ");
double distance = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Введите средний расход топлива на 100 км (л): ");
double consumptionPer100 = Convert.ToDouble(Console.ReadLine());

Console.WriteLine("Введите стоимость литра бензина: ");
decimal pricePerLiter = Convert.ToDecimal(Console.ReadLine());

double liters = distance * consumptionPer100 / 100;
decimal totalCost = (decimal)liters * pricePerLiter;

Console.WriteLine();
Console.WriteLine($"Необходимо литров: {liters:F2}");
Console.WriteLine($"Итоговые затраты: {totalCost:F2}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program42.png">
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
//Побитовые маски и права доступа: Задайте константы флагов доступа (Read = 1, Write = 2, Execute = 4). Считайте целое число от 0 до 7 и выведите список доступных прав, используя побитовое И (&).

 Console.Clear();
 Console.ForegroundColor = ConsoleColor.DarkGreen;
 Console.WriteLine("Побитовые маски и права доступа");
 Console.ForegroundColor = ConsoleColor.Gray;

 const int Read = 1;
 const int Write = 2;
 const int Execute = 4;

 Console.WriteLine("Введите число от 0 до 7: ");
 int name12 = Convert.ToInt32(Console.ReadLine());

 Console.WriteLine("Доступные права:");

 if ((name12 & Read) == Read)
     Console.WriteLine("Read");
 if ((name12 & Write) == Write)
     Console.WriteLine("Write");
 if ((name12 & Execute) == Execute)
     Console.WriteLine("Execute");
 if (name12 == 0)
     Console.WriteLine("Нет прав доступа");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program43.png">
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
 //Форматирование вывода сводной таблицы: Считайте данные об успеваемости трех студентов (ФИО, курс, средний балл). Выведите аккуратную отформатированную таблицу с фиксированной шириной столбцов, используя форматирование строк: Console.WriteLine("{0,-20} {1,5} {2,8:F2}", ...);.


            Console.WriteLine("Сводная таблица успеваемости");


            Console.WriteLine("Введите ФИО первого студента: ");
            string name13 = Console.ReadLine();
            Console.WriteLine("Введите курс первого студента: ");
            int name14 = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Введите средний балл первого студента: ");
            double name15 = Convert.ToDouble(Console.ReadLine());

            Console.WriteLine("Введите ФИО второго студента: ");
            string name16 = Console.ReadLine();
            Console.WriteLine("Введите курс второго студента: ");
            int name17 = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Введите средний балл второго студента: ");
            double name18 = Convert.ToDouble(Console.ReadLine());

            Console.WriteLine("Введите ФИО третьего студента: ");
            string name19 = Console.ReadLine();
            Console.WriteLine("Введите курс третьего студента: ");
            int name20 = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Введите средний балл третьего студента: ");
            double name21 = Convert.ToDouble(Console.ReadLine());

            Console.WriteLine();
            Console.WriteLine("{0,-20} {1,5} {2,8}", "ФИО", "Курс", "Балл");
            Console.WriteLine(new string('-', 36));

            Console.WriteLine("{0,-20} {1,5} {2,8:F2}", name13, name14, name15);
            Console.WriteLine("{0,-20} {1,5} {2,8:F2}", name16, name17, name18);
            Console.WriteLine("{0,-20} {1,5} {2,8:F2}", name19, name20, name21);

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program44.png">
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
//Шифрование одного символа: Запросите у пользователя символ и секретный ключ (целое число от 1 до 255). Выполните операцию XOR (^) над кодом символа и ключом, выведите зашифрованный символ и его код. Повторите операцию с тем же ключом, показав расшифровку исходного символа.


            Console.WriteLine("Шифрование одного символа с помощью XOR");


            Console.WriteLine("Введите символ: ");
            char name22 = Convert.ToChar(Console.ReadLine());

            Console.WriteLine("Введите секретный ключ (1–255): ");
            int name23 = Convert.ToInt32(Console.ReadLine());

            char name24 = (char)(name22 ^ name23);
            Console.WriteLine($"Зашифрованный символ: {name24}");
            Console.WriteLine($"Код зашифрованного символа: {(int)name24}");

            char name25 = (char)(name24 ^ name23);
            Console.WriteLine($"Расшифрованный символ: {name25}");
            Console.WriteLine($"Код расшифрованного символа: {(int)name25}");

        }
    }
}

```
`Результат выполнения:`
<picture>
  <img src="https://github.com/KseniaBashkatova/3ve3dochka/blob/main/assets/screens/Program45.png">
</picture>
```
🧑‍💻 Ссылка на практическую работу №1 и преподавателя [github](https://github.com/U5er01Task/Fundamentals-of-Algorithmization-and-Programming-2026/tree/main) - [Преподаватель](https://github.com/U5er01Task)

---
