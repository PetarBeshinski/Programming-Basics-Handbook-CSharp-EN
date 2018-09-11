#### Преброяване на биковете и кравите

Каква логика можем да използваме? Най-елементарният начин да проверим колко крави и бикове има в едно число е чрез **поредица от `if-else` проверки**. Да, не е най-оптималния начин, но с цел да не използваме знания извън пределите на тази книга, ще изберем този подход.

От какви проверки имаме нужда?

Проверката за бикове е елементарна - проверяваме дали **първата цифра** от генерираното число е еднаква със **същата цифра** от секретното число. Премахваме проверените цифри с цел да избегнем повторения на бикове и крави.

![](/assets/chapter-9-2-images/03.Bulls-and-cows-09.png)

Повтаряме действието за втората, третата и четвърта цифра. 

Проверката за крави можем да направи по следния начин - първо проверяваме дали **първата цифра** от генерираното число **съвпада с втората**, **третата** или **четвъртата цифра** на секретното число. Примерна имплементация:

![](/assets/chapter-9-2-images/03.Bulls-and-cows-10.png)

След това последователно проверяваме дали **втората цифра** от генерираното число **съвпада с първата**, **третата** или **четвъртата цифра** на секретното число, дали **третата цифра** от генерираното число съвпада с **първата**, **втората** или **четвъртата цифра** на секретното число и накрая проверяваме дали **четвъртата цифра** от генерираното число съвпада с **първата**, **втората** или **третата цифра** на секретното число.