# RomanIntegerCalculator
## RU
### Описание:
Создай консольное приложение “Калькулятор”. Приложение должно читать из консоли введенные пользователем строки, числа, арифметические операции проводимые между ними и выводить в консоль результат их выполнения.
Реализуй класс Main с методом public static String calc(String input). Метод должен принимать строку с арифметическим выражением между двумя числами и возвращать строку с результатом их выполнения. Ты можешь добавлять свои импорты, классы и методы. Добавленные классы не должны иметь модификаторы доступа (public или другие)
### Требования:
1. Калькулятор умеет выполнять операции сложения, вычитания, умножения и деления с двумя числами: a + b, a - b, a * b, a / b. Данные передаются в одну строку (смотри пример)! Решения, в которых каждое число и арифмитеческая операция передаются с новой строки считаются неверными.
2. Калькулятор умеет работать как с арабскими (1,2,3,4,5…), так и с римскими (I,II,III,IV,V…) числами.
3. Калькулятор должен принимать на вход числа от 1 до 10 включительно, не более. На выходе числа не ограничиваются по величине и могут быть любыми.
4. Калькулятор умеет работать только с целыми числами.
5. Калькулятор умеет работать только с арабскими или римскими цифрами одновременно, при вводе пользователем строки вроде 3 + II калькулятор должен выбросить исключение и прекратить свою работу.
6. При вводе римских чисел, ответ должен быть выведен римскими цифрами, соответственно, при вводе арабских - ответ ожидается арабскими.
7. При вводе пользователем неподходящих чисел приложение выбрасывает исключение и завершает свою работу.
8. При вводе пользователем строки, не соответствующей одной из вышеописанных арифметических операций, приложение выбрасывает исключение и завершает свою работу.
9. Результатом операции деления является целое число, остаток отбрасывается. 
10. Результатом работы калькулятора с арабскими числами могут быть отрицательные числа и ноль. Результатом работы калькулятора с римскими числами могут быть только положительные числа, если результат работы меньше единицы, выбрасывается исключение
### Реализация решения:
Для проверки строки на условие наличия в ней арабских цифр использовал регулярные выражения. Для проверки на наличие римских - сплитил строку с сепаратором в виде оператора и проверял полученный массив, римские ли в нем или нет.
Реализация калькулятора достаточно проста, использовал if-else конструкции.
## ENG
### Description:
Create a "Calculator" console application. The application must read from the console the strings, numbers, arithmetic operations between them and output the result to the console.
Implement class Main with method public static String calc(String input). The method should accept a string with an arithmetic expression between the two numbers and return a string with the result of their execution. You can add your own imports, classes, and methods. Added classes must not have access modifiers (public or otherwise)
#### Requirements:
1. The calculator can perform addition, subtraction, multiplication and division operations with two numbers: a + b, a - b, a * b, a / b. The data is transmitted in one line (see example)! Solutions in which each number and arithmetic operation is passed from a new line are considered incorrect.
2. The calculator can work both with Arabic (1,2,3,4,5...) and Roman (I,II,III,IV,V...) numbers.
3. The calculator should be able to accept numbers from 1 to 10 inclusive. The output numbers are not limited in size and may be any.
4. The calculator can only work with integers.
5. The calculator can only work with Arabic or Roman numerals at a time, if the user enters a string like 3 + II the calculator must throw an exception and stop its work.
6. When entering Roman numbers, the answer should be printed in Roman numerals, respectively, when entering Arabic numerals, the answer is expected in Arabic numerals.
7. If the user enters unsuitable numbers, the application throws an exception and stops its work.
8. If the user enters a string that does not match one of the arithmetic operations described above, the application throws an exception and terminates.
9. The result of a division operation is an integer, the remainder is discarded. 
10. The result of the calculator operations with Arabic numbers can be negative numbers and zero. The result of the calculator with Roman numbers can only be positive numbers, if the result is less than one, an exception is thrown
### Implementation of the solution:
Used regular expressions to check the string for the condition that it contains Arabic digits. To check for the presence of Roman numerals, I split the string with the separator as an operator and checked the resulting array to see if it contained Roman numerals or not.
Implementation of the calculator is simple enough, I used if-else constructions.
