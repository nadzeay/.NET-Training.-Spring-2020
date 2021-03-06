## Читать
- [C# 6.0 in a Nutshell. Joseph Albahari, Ben Albahari. O'Reilly Media. 2015.](https://drive.google.com/drive/u/0/folders/0B7WmjuqYed3Aeko0MzNYZWtVOUk)
   - *Chapter 3.* Creating Types in C#
- [C# 5.0 Unleashed. Bart De Smet. Sams Publishing. 2013.](https://drive.google.com/drive/u/0/folders/0B7WmjuqYed3Aeko0MzNYZWtVOUk)
   - *Chapter 9.* Introducing Types

## Материалы (презентация)
- [Basic Coding in C#](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M4.%20Methods%20in%20details)
- [Creating types in C#](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M3.%20Creating%20types%20in%20C%23)

## Задачи (Day 4 - Day 5)
 
1. **(deadline 29.03.2019, 24.00)** Реализовать класс Transformer, метод TransformToWords которого выполняет преобразование System.Double в его "словестный формат". Например, -23.809 -> "minus two three point eight zero nine". Разработать модульные тесты для тестирования метода.
2. **(deadline 29.03.2019, 24.00)** Расширить функциональную возможность типа System.Double, реализовав метод Transform, который принимает массив вещественных чисел и трансформирует его в массив строк таким образом, чтобы каждое вещественное число преобразовывалось в его "словестный формат" (LINQ-запросы не использовать!). Например, {-23.809, 0.295, 15.17} -> {"minus two three point eight zero nine", "zero point two nine five", "one five point one seven"}. Разработать модульные тесты для тестирования метода.
3. **(deadline 30.03.2019, 24.00)** Расширить функциональную возможность типа System.Double, реализовав возможность получения строкового представления вещественного числа в формате IEEE 754. *Готовые классы-конверторы не использовать.* Разработать модульные тесты. Примерные тест-кейсы (для тестирования специальных значений вещественных чисел возможны варианты)
    - [TestCase(-255.255, ExpectedResult = "1100000001101111111010000010100011110101110000101000111101011100")]
    - [TestCase(255.255, ExpectedResult = "0100000001101111111010000010100011110101110000101000111101011100")]
    - [TestCase(4294967295.0, ExpectedResult = "0100000111101111111111111111111111111111111000000000000000000000")]
    - [TestCase(double.MinValue, ExpectedResult = "1111111111101111111111111111111111111111111111111111111111111111")]
    - [TestCase(double.MaxValue, ExpectedResult = "0111111111101111111111111111111111111111111111111111111111111111")]
    - [TestCase(double.Epsilon, ExpectedResult = "0000000000000000000000000000000000000000000000000000000000000001")]
    - [TestCase(double.NaN, ExpectedResult = "1111111111111000000000000000000000000000000000000000000000000000")]
    - [TestCase(double.NegativeInfinity, ExpectedResult = "1111111111110000000000000000000000000000000000000000000000000000")]
    - [TestCase(double.PositiveInfinity, ExpectedResult = "0111111111110000000000000000000000000000000000000000000000000000")]
    - [TestCase(-0.0, ExpectedResult = "1000000000000000000000000000000000000000000000000000000000000000")]
    - [TestCase(0.0, ExpectedResult = "0000000000000000000000000000000000000000000000000000000000000000")] 
     и т.д.
     
     **(deadline 02.03.2019)** Добавить ASP.NET MVC пользовательский интерфейс для работы с разработанной логикой.  
4. **(deadline 31.03.2019, 24.00)** Разработать неизменяемый класс Polynomial (полином) для работы с многочленами *n*-ой степени от одной переменной вещественного типа (в качестве внутренней структуры для хранения коэффициентов использовать sz-массив). Для разработанного класса переопределить виртуальные методы класса Object; перегрузить операции, допустимые для работы с многочленами (исключая деление многочлена на многочлен), включая "==" и "!=". Разработать модульные тесты для тестирования методов класса.
