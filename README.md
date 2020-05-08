# Отчёт о тестировании кода

## Краткое описание

07.05.2020 было проведено тестирование кода в IntelliJ IDEA. Тестировался функционал проверки валидации номера карты.

На тестирование затрачено: 1 час

В результате тестирования выявлены следующие валидные номера кредитных карт не прошедшие валидацию:
* VISA:
4485141125341962474
* American Express (AMEX):
376308961561597,
346893889881331,
344353741132458
* Discover:
6011109386457512543
* JCB:
3542465607537776096
* Diners Club - Carte Blanche:
30541165725125,
30253980267487,
30204249666985
* Diners Club - International:
36626649969557,
36174544135560,
36062766614828

!!!ВАЖНОЕ НАБЛЮДЕНИЕ!!!
* На валидность не прошли валидные номера карт, в которых было либо меньше, либо больше 17 цифр. Карты состоящие из 17 цифр все оказались валидными.

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* Отчет о прохождении тестирования
* Issue

Далее приведены результаты тестирования на наборе тестовых данных::

VISA:
- 4539033247387791 - OK
- 4716646850281616 - OK
- 4485141125341962474 - FAIL

MasterCard:
- 5211034561412720 - OK
- 2221001368440597 - OK
- 5111956528828732 - OK

American Express (AMEX):
- 376308961561597 - FAIL
- 346893889881331 - FAIL
- 344353741132458 - FAIL

Discover:
- 6011350409537803 - OK
- 6011846966995904 - OK
- 6011109386457512543 - FAIL

JCB:
- 3529467089808007 - OK
- 3545115796143966 - OK
- 3542465607537776096 - FAIL

Diners Club - North America:
- 5447940671504006 - OK
- 5531354831249097 - OK
- 5439781640110875 - OK

Diners Club - Carte Blanche:
- 30541165725125 - FAIL
- 30253980267487 - FAIL
- 30204249666985 - FAIL

Diners Club - International:
- 36626649969557 - FAIL
- 36174544135560 - FAIL
- 36062766614828 - FAIL

Maestro:
- 0604578217017321 - OK
- 5038059007080048 - OK
- 5020087448718959 - OK

Visa Electron:
- 4913438036213783 - OK
- 4917463514299449 - OK
- 4917457519170142 - OK

InstaPayment:
- 6377534622146074 - OK
- 6376172742734189 - OK
- 6383828444355208 - OK

Ожидаемый результат:
* Result is OK

Фактический результат:
* Некоторые валидные номера карт не прошли проверку на валидность, по ним заведено issue в репозитории https://github.com/tatiana-polyakova/Credit-Card-Number-Validator

На валидность не прошли валидные номера карт, в которых было либо меньше, либо больше 17 цифр. Карты состоящие из 17 цифр все оказались валидными.

Тестирование производилось в следующем окружении:

* Устройство: Ноутбук Xiaomi
* ОС: Windows 10 Pro
* openjdk version "11.0.7" 2020-04-14
* OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.7+10)
* OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.7+10, mixed mode)