# Отчёт о тестировании Credit Card Number Validator #  

### Краткое описание ###  

<29.01.2021> - <29.01.2021> было проведено <функциональное тестировние> приложения Credit Card Number Validator  

На тестирование затрачено: <2 часа>  

#### В результате тестирования было выявлено следущее: ####  

[Программа считает валидные номера карт American Express (AMEX) невалидными][4]  
[Программа считает валидные номера карт Diners Club - Carte Blanche невалидными][5]  

### Описание процесса тестирования ###  

В качестве тестовых данных использовались данные [www.freeformatter.com][1] 

#### VISA: ####    

4539900177748509  
ОР: Result is OK  
ФР: Result is OK  
4024007100321149  
ОР: Result is OK  
ФР: Result is OK  
4716135683123481697  
ОР: Result is FAIL  
ФР: Result is FAIL  

#### MasterCard: ###  

5525816089112647  
ОР: Result is OK    
ФР: Result is OK      
5210259612627478  
ОР: Result is OK  
ФР: Result is OK    
5431502031762647  
ОР: Result is OK  
ФР: Result is OK    

#### American Express (AMEX): ####  

340210322597992  
ОР: Result is OK    
ФР: Result is FAIL     
343621645199836  
ОР: Result is OK    
ФР: Result is FAIL  
374629892469317  
ОР: Result is OK    
ФР: Result is FAIL  

#### Diners Club - Carte Blanche: ####  
30370706552560  
ОР: Result is OK    
ФР: Result is FAIL  
30078960263028  
ОР: Result is OK    
ФР: Result is FAIL  
30247836519919  
ОР: Result is OK    
ФР: Result is FAIL  

#### MIR ####
2201382000000013  
ОР: Result is OK    
ФР: Result is OK  
2201382000000013  
ОР: Result is OK      
ФР: Result is OK  
      

**В результате тестирования выявлены следующие дефекты:**    

1. [Не валидныe номерf карт American Express (AMEX)][2]
1. [Не валидные номера карты Diners Club - Carte Blanche][3]  

### Тестирование производилось в следующем окружении: ###    

<Windows 10 Домашняя Версия 2004, Разрядность - 64>  
<версия Java openjdk 11.0.10 2021-01-19>  
<IntelliJ IDEA Community Edition 2020.3.2 x64>  

[1]: https://www.freeformatter.com/credit-card-number-generator-validator.html    
[2]: https://github.com/AnnaStarkov/DZJ1.1.2/issues/4#issue-796822596
[3]: https://github.com/AnnaStarkov/DZJ1.1.2/issues/5#issue-796833113
[4]: https://github.com/AnnaStarkov/DZJ1.1.2/issues/4#issue-796822596 
[5]: https://github.com/AnnaStarkov/DZJ1.1.2/issues/5#issue-796833113  