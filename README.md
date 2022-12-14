# Test

## Введение

Этот документ описывает тестирование проекта "Determination properties of numbers"

## 1  Описание тестирования

### 1.1  План тестирования

Этот план тестирования описывает подход к тестированию, который мы использовали для тестирования проекта.

В документе представлены:
Цель тестирования: описывают задачи которые должны выполнять тесты

Требования к тестированию: правила, на которых будет основано тестирование, и описание процесса тестирования.

Функциональное тестирование: Проверка работы функциональностей программы.

### 1.2 Описание проекта

"Determination properties of numbers" это веб приложение для определение свойств чисел.

Приложение считывает значение введенного пользователем число, после чего выводит на экран результат в виде строки с данными.

## 2 Стратегия тестирования

### 2.1 Цель тестирования

Цель тестов:
-убедиться что функциональное генерирование правильности опрделения свойств происходит верно и работает в соответствии с составленной спецификацией

-убедиться что функциональное генерирование ответа на ошибочный ввод(отриательное число) происходит верно и работает в соответствии с составленной спецификацией

-убедиться что функциональное генерирование ответа на ошибочный ввод(не целое число и другие символы) происходит верно и работает в соответствии с составленной спецификацией

Тесты будет представлены отдельным файлом который мы можем запустить отдельно от приложения.

Конечным продуктом тестов является автономное веб приложение, которое будет использоваться для разработки стабильного программного обеспечения и поможет программистам убедиться в отсутствии критических ошибок в алгоритмах.

### 2.2 Требования к тестированию

1)Первый тест будет сосредоточен на проверке алгоритма правильности определения свойств чисел введенных пользователем.
Процесс тестирования будет максимально гибким, чтобы обеспечить возможность его расширения для новых алгоритмов и тестовых случаев.
Тесты будут создаваться как отдельное файл программы, чтобы обеспечить понятную структуризацию проекта, повысить скорость его сборки и минимизировать количество неиспользуемого кода.
Тестовая среда и данные будут максимально эмулировать производственные.
Тестирование будет использовать предварительно загруженные реальные данные, которые могут и будут использоваться в реальном конечном продукте.


2)Второй тест будет сосредоточен на генерации ответа на ошибочный ввод(отриательное число).
Процесс тестирования будет максимально гибким, чтобы обеспечить возможность его расширения для новых алгоритмов и тестовых случаев.
Тесты будут создаваться как отдельное приложение, чтобы обеспечить понятную структуризацию проекта, повысить скорость его сборки и минимизировать количество неиспользуемого кода.
Тестовая среда и данные будут максимально эмулировать производственные.
Тестирование будет использовать предварительно загруженные реальные данные, которые могут и будут использоваться в реальном конечном продукте.


3)Третий тест будет сосредоточен на генерации ответа на ошибочный ввод(не целое число и другие символы).
Процесс тестирования будет максимально гибким, чтобы обеспечить возможность его расширения для новых алгоритмов и тестовых случаев.
Тесты будут создаваться как отдельное приложение, чтобы обеспечить понятную структуризацию проекта, повысить скорость его сборки и минимизировать количество неиспользуемого кода.
Тестовая среда и данные будут максимально эмулировать производственные.
Тестирование будет использовать предварительно загруженные реальные данные, которые могут и будут использоваться в реальном конечном продукте.

### 2.3 Функциональное тестирование

**Цель:** проверить функции приложения. Функциональное тестирование выполняется путем подачи входных данных и проверки выходных данных приложения.

**Метод:** тест будет использовать предварительно загруженные данные (входные и ожидаемые выходные данные) для проверки вывода функций из разных входных данных.

**Критерии приемлемости теста:** пройти, если результат функции такой же, как и ожидалось, иначе - не пройти.

**Сроки:** единственное требование здесь — не допускать вечных циклов.

### 2.3.1 Тестирование алгоритма функции "Определение свойств чисел"

Тест " positiveTest " не принимает входных значений, вызывает методы программы и сравнивает фактический и ожидаемый результаты и выводит соответствующий ответ.  

![](https://github.com/NAsQuk/TRITPO_6/blob/main/TESTS/теск%20кейс%20ответ%20на%20запрос%20польз._1.png)

### 2.3.2 Тестирование алгоритма функции "Генерация ответа н аошибочный ввод"

Тест " handleMethodArgumentTypeMismatchExeption " не принимает входных значений, вызывает методы программы и сравнивает фактический и ожидаемый результаты и выводит соответствующий ответ. 

![](https://github.com/NAsQuk/TRITPO_6/blob/main/TESTS/тест-комплект%20ошибка_1.png)
![](https://github.com/NAsQuk/TRITPO_6/blob/main/TESTS/тест-комплект%20ошибка_2.png)

### 2.4 Нагрузочное тестирование

Нагрузочное тестирование было проведено при помощи утилиты Postman.
Были написаны тесты для определения работоспособности приложения при сильной нагруженности сайта.

## 3 Среда тестирования

ОС:

MAC OS, Windows, Linux

Язык программирования и библиотеки:

Среда разработки и тестирования: IntelliJ IDEA 2021.3.2

Среда для нагрузочного тестирования: Postman

Язык программирования: Java 17.0.2

Средство тестирования: Java Unit Tests
