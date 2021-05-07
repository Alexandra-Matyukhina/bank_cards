# Отчёт о тестировании функциональности валидации номера банковской карты

## Краткое описание

<2021.05.07 at 7:00 PM> - <2021.05.07 at 8:00 PM> было проведено тестирование функциональности валидации номера банковской карты методом Black Box, а именно ввод граничных и эквивалентных значений.

На тестирование затрачено: <1 час>

В результате тестирования выявлены следующие дефекты:
* https://github.com/Alexandra-Matyukhina/bank_cards/issues/4#issue-879509435
* https://github.com/Alexandra-Matyukhina/bank_cards/issues/3#issue-879480330
* https://github.com/Alexandra-Matyukhina/bank_cards/issues/2#issue-879418634

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:
* Баг-Репорты
* Отчет о тестировании


В качестве тестовых данных использовались данные https://www.freeformatter.com/credit-card-number-generator-validator.html:
* VISA:
4929529336278898 - Expected Result - Result is OK
4716987144875296 - Expected Result - Result is OK
4929850532395190613 - Expected Result - Result is OK
* MasterCard:
5501396643328391 - Expected Result - Result is OK
5557177243148162 - Expected Result - Result is OK
5313515700543786 - Expected Result - Result is OK
* American Express (AMEX):
374848875562639 - Expected Result - Result is OK
375215114122766 - Expected Result - Result is OK
345425572667189 - Expected Result - Result is OK
* Discover:
6011295331572131 - Expected Result - Result is OK
6011000363538962 - Expected Result - Result is OK
6011236665624590839 - Expected Result - Result is OK
* JCB:
3541651461967119 - Expected Result - Result is OK
3589846340699700 - Expected Result - Result is OK
3539551324211706412 - Expected Result - Result is OK
* Diners Club - North America:
5421483127513362 - Expected Result - Result is OK
5438388790981021 - Expected Result - Result is OK
5497433331336372 - Expected Result - Result is OK
* Diners Club - Carte Blanche:
30004606777940 - Expected Result - Result is OK
30028395433662 - Expected Result - Result is OK
30406894563140 - Expected Result - Result is OK
* Diners Club - International:
36760638022753 - Expected Result - Result is OK
36742541948563 - Expected Result - Result is OK
36110394568708 - Expected Result - Result is OK
* Maestro:
6304183947768226 - Expected Result - Result is OK
5893692921489806 - Expected Result - Result is OK
6759280277466551 - Expected Result - Result is OK
* Visa Electron:
4026922281239084 - Expected Result - Result is OK
4917073427551362 - Expected Result - Result is OK
4917326384458462 - Expected Result - Result is OK
* InstaPayment:
6372861798014363 - Expected Result - Result is OK
6389414085475193 - Expected Result - Result is OK
6380402633845792 - Expected Result - Result is OK


Тестирование производилось в следующем окружении:
* Устройство: Microsoft Surface Laptop 3
* Windows 10
* AdoptOpenJDK JDK with Hotspot 11.0.10+9 (x64)
* IntelliJ IDEA 2021.1.1 (Community Edition), Runtime version: 11.0.10+9-b1341.41 amd64)