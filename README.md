# Отчёт о тестировании <Название приложения>

## Краткое описание

02.05.2020 было проведено тестирование кода в IntelliJ IDEA.

На тестирование затрачено: 1 час

В результате тестирования выявлены следующие дефекты:
* https://github.com/tatiana-polyakova/Credit-Card-Number-Validator/blob/master/%D0%91%D0%B0%D0%B3%20%D1%81%20VISA.png?raw=true
* https://github.com/tatiana-polyakova/Credit-Card-Number-Validator/blob/master/%D0%91%D0%B0%D0%B3%20%D1%81%20JCB.png?raw=true
* https://github.com/tatiana-polyakova/Credit-Card-Number-Validator/blob/master/%D0%91%D0%B0%D0%B3%20%D1%81%20Discover.png?raw=true
* https://github.com/tatiana-polyakova/Credit-Card-Number-Validator/blob/master/%D0%91%D0%B0%D0%B3%20%D1%81%20Diners%20Club%20-%20International.png?raw=true
* https://github.com/tatiana-polyakova/Credit-Card-Number-Validator/blob/master/%D0%91%D0%B0%D0%B3%20%D1%81%20Diners%20Club%20-%20Carte%20Blanche.png?raw=true
* https://github.com/tatiana-polyakova/Credit-Card-Number-Validator/blob/master/%D0%91%D0%B0%D0%B3%20%D1%81%20American%20Express%20(AMEX).png?raw=true


## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* Номера карт созданные на сайте https://www.freeformatter.com/
* IntelliJ IDEA
* Paint


В качестве тестовых данных использовались данные карт с сайта https://www.freeformatter.com:
* Номера карт для теста - https://github.com/tatiana-polyakova/Credit-Card-Number-Validator/blob/master/%D0%9D%D0%BE%D0%BC%D0%B5%D1%80%D0%B0%20%D0%BA%D0%B0%D1%80%D1%82.png?raw=true

Ожидаемый результат:
* Result is OK

Фактический результат:
* Некоторые из номеров карт не прошли проверку, по ним я завела issues в репозитории https://github.com/tatiana-polyakova/Credit-Card-Number-Validator

Тестирование производилось в следующем окружении:

* Устройство: Ноутбук Xiaomi
* ОС: Windows 10 Pro
* openjdk version "11.0.7" 2020-04-14
* OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.7+10)
* OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.7+10, mixed mode)