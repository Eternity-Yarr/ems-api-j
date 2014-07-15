ems-api-j
=========

Простой модуль для расчета стоимости EMS почты России через API http://emspost.ru/ru/corp_clients/dogovor_docements/api/


Использование:

```java
EMSService es = new EMSService();
Location from = es.findLocation("Москва");
Location to = es.findLocation("Воронеж");
int price = es.getPrice(from, to, 5); // price == 790
```