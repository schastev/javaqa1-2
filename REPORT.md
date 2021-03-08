# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

7.03.2021 было проведено функциональное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 2 ч.

В результате тестирования выявлены следующие дефекты:
* [Номера карт, состоящие не из 16 цифр, не распознаются как валидные](https://github.com/k-emiko/javaqa1-2/issues/1)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* https://github.com/netology-code/javaqa-homeworks/tree/master/intro

В качестве тестовых данных использовались данные [freeformatter](https://www.freeformatter.com/credit-card-number-generator-validator.html#fakeNumbers) и [saijogeorge](https://saijogeorge.com/dummy-credit-card-generator/):
* 4174191298081 - OK X
* 4929398289810697 - OK
* 4133245383719347585 - OK  X
* 5324335391186762 - OK
* 5242573603819403 - OK
* 343431775253795 - OK X
* 6011535954327523 - OK
* 6011111070539423 - OK
* 6011222455906968648 - OK X
* 3544515603844105 - OK
* 3529914629903384994 - OK X
* 5433031970334836 - OK
* 30125860504751 - OK X
* 30474009457822 - OK X
* 36521577185385 - OK X
* 36907304161288 - OK X
* 0604939247576217 - OK
* 5020814255793050 - OK
* 351488654876269 - ОК X
* 6011976576243047 - OK
* 5296126987052383 - OK
* 4859404581771134 - OK

Тестирование производилось в следующем окружении:
* LMDE 4 Debbie, kernel 4.19.0-13-amd64
* openjdk version "11.0.9.1" 2020-11-04
* OpenJDK Runtime Environment (build 11.0.9.1+1-post-Debian-1deb10u2)
* OpenJDK 64-Bit Server VM (build 11.0.9.1+1-post-Debian-1deb10u2, mixed mode, sharing)