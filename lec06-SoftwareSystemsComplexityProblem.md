# Software Systems Complexity Problem (лекция 6)

Пара цитат по теме:
- Основная проблема программиста: не сломаться из-за сложности своего же кода
- Управление сложностью - самая важная техническая тема в мире разработки программиного обеспечения
- Сегодня в программирование точно те же проблемы как и 50 лет назад: как поддерживать контроль над кодом с большой сложностью
- **Наибольший барьер в написании софта: это ограниченность понимания систем, которые мы создаем**

Вещи с наибольшим вкладом в сложность кода
- **сам код** - основная проблема
- отсутствующая или неправильная документация
- сложный UI
- ...

Диаграмма скорости написания новой логики от времени жизни проекта:
![image](https://user-images.githubusercontent.com/57497898/212562715-d96d1b65-9da9-4a98-9297-039ff3774a6c.png)

Сложность аккумулируется. То есть код может быть сложным, даже если в нем есть много маленьких усложнений, которые почти никак не мешают сами по себе

Сложность делает разработку более долгой и пораждает баги, которые так же замедляют разработку

![image](https://user-images.githubusercontent.com/57497898/213713970-8b3c6270-5020-473c-9aa7-e0ac58b9d1b3.png)

В итоге проект рано или поздно перестанет развиваться, так как развитие начнет обходиться слишком накладно

(это небольшая проблема когда у вас маленький проект)

Допустим вы оказались в такой ситуации когда проект развивается очень долго. Тогда вы можете захотеть нанять больше людей. Но если вы наймете слишком много людей, то только проиграете по времени. 

График зависимости скорости написания новой логики от количества разработчиков:
![image](https://user-images.githubusercontent.com/57497898/212563604-dee033cf-05e7-4c88-be3e-d54afdebdcc6.png)

Вывод сложность кодовой базы не всегда решается деньгами. Порой нет хороших решений. А те что есть (рефакторинг или переписывание с нуля), очень дорогие по времени

Поэтому надо поощрять программистов писать хороший код. Хорошие разработчики и культура правильного кода увеличивает время жизни и качество проекта

Тем не менее три способа бороться со сложной кодовой базой:
- нанять еще сотрудников
- рефакторинг существующего кода
- переписывание кода

----
## 10x разработчик

Существуют разработчики, которые в разы более продуктивны. 

- Они отличаются от остальных тем, что они понимают систему над которой работают.
Есть очень старые кодовые базы, где существет код в котором никто из команды уже не может разобраться. Если поместить в такую продуктивного разработчика, то он перестанет быть таким продуктивным
- Они оставляют разрабатываемую систему простой (чем повышают продуктивность всей команды)

---- 

## Управление сложностью

Управлять сложностью проекта - это искусство
- важно иметь талант
- нужно постоянно практиковаться (например с помошью фидбеков на ревью или наблюдая за своим старым кодом)
- имеется теория, которую лучше изучить

Пытайтесь минимизировать сложность на всех уровнях разработки вашего проекта