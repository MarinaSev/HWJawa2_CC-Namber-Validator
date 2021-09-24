# Отчёт о тестировании приложения Credit Card Number Validator

## Краткое описание

13.09.2021 было проведено дымовое ситемное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 0,25 часа

В результате тестирования выявлено следующее:
* система принимает карты с 16-тизначным номером (Visa, MasterCard, Discover - OK;
* [система не принимает карты AmEx](https://github.com/MarinaSev/HWJawa2_CC-Namber-Validator/issues/1#issue-1006686162) (у них 15 цифр в номере) - *требует доработки, если планируется приём карт American Express*;
* система не принимает номера карт, содержащие меньше или больше 16-ти цифр - OK;
* система не принимает случайный набор из 16-ти цифр - OK.

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* [Исходные данные из Задачи №2 - Credit Card Number Validator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/MERGED.md)

В качестве тестовых данных использовались данные:
* [Код из Задачи №2 - Credit Card Number Validator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/MERGED.md)
* [Номера кредитных карт, сгенерированных на Get Credit Card Numbers Generator](https://www.getcreditcardnumbers.com/)

Тестирование производилось в следующем окружении:
* Windows10 (2004), х64
* OpenJDK version "11.0.12" 2021-07-20
