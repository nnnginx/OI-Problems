## Description

<div><p>Завтра у хоккейной команды, которой руководит Евгений, важный матч. Евгению нужно выбрать шесть игроков, которые выйдут на лед в стартовом составе: один вратарь, два защитника и три нападающих.</p><p>Так как это стартовый состав, Евгения больше волнует, насколько красива будет команда на льду, чем способности игроков. А именно, Евгений хочет выбрать такой стартовый состав, чтобы номера любых двух игроков из стартового состава отличались не более, чем в два раза. Например, игроки с номерами <span class="tex-span">13</span>, <span class="tex-span">14</span>, <span class="tex-span">10</span>, <span class="tex-span">18</span>, <span class="tex-span">15</span> и <span class="tex-span">20</span> устроят Евгения, а если, например, на лед выйдут игроки с номерами <span class="tex-span">8</span> и <span class="tex-span">17</span>, то это не устроит Евгения.</p><p>Про каждого из игроков вам известно, на какой позиции он играет (вратарь, защитник или нападающий), а также его номер. В хоккее номера игроков не обязательно идут подряд. Посчитайте число различных стартовых составов из одного вратаря, двух защитников и трех нападающих, которые может выбрать Евгений, чтобы выполнялось его условие красоты.</p></div><div class="input-specification"><p>Первая строка содержит три целых числа <span class="tex-span"><i>g</i></span>, <span class="tex-span"><i>d</i></span> и <span class="tex-span"><i>f</i></span> (<span class="tex-span">1 ≤ <i>g</i> ≤ 1 000</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 1 000</span>, <span class="tex-span">1 ≤ <i>f</i> ≤ 1 000</span>)&nbsp;— число вратарей, защитников и нападающих в команде Евгения. </p><p>Вторая строка содержит <span class="tex-span"><i>g</i></span> целых чисел, каждое в пределах от <span class="tex-span">1</span> до <span class="tex-span">100 000</span>&nbsp;— номера вратарей.</p><p>Третья строка содержит <span class="tex-span"><i>d</i></span> целых чисел, каждое в пределах от <span class="tex-span">1</span> до <span class="tex-span">100 000</span>&nbsp;— номера защитников.</p><p>Четвертая строка содержит <span class="tex-span"><i>f</i></span> целых чисел, каждое в пределах от <span class="tex-span">1</span> до <span class="tex-span">100 000</span>&nbsp;— номера нападающих.</p><p>Гарантируется, что общее количество игроков не превосходит <span class="tex-span">1 000</span>, т.&nbsp;е. <span class="tex-span"><i>g</i> + <i>d</i> + <i>f</i> ≤ 1 000</span>. Все <span class="tex-span"><i>g</i> + <i>d</i> + <i>f</i></span> номеров игроков различны.</p></div><div class="output-specification"><p>Выведите одно целое число&nbsp;— количество возможных стартовых составов.</p></div>

## Input

<p>Первая строка содержит три целых числа <span class="tex-span"><i>g</i></span>, <span class="tex-span"><i>d</i></span> и <span class="tex-span"><i>f</i></span> (<span class="tex-span">1 ≤ <i>g</i> ≤ 1 000</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 1 000</span>, <span class="tex-span">1 ≤ <i>f</i> ≤ 1 000</span>)&nbsp;— число вратарей, защитников и нападающих в команде Евгения. </p><p>Вторая строка содержит <span class="tex-span"><i>g</i></span> целых чисел, каждое в пределах от <span class="tex-span">1</span> до <span class="tex-span">100 000</span>&nbsp;— номера вратарей.</p><p>Третья строка содержит <span class="tex-span"><i>d</i></span> целых чисел, каждое в пределах от <span class="tex-span">1</span> до <span class="tex-span">100 000</span>&nbsp;— номера защитников.</p><p>Четвертая строка содержит <span class="tex-span"><i>f</i></span> целых чисел, каждое в пределах от <span class="tex-span">1</span> до <span class="tex-span">100 000</span>&nbsp;— номера нападающих.</p><p>Гарантируется, что общее количество игроков не превосходит <span class="tex-span">1 000</span>, т.&nbsp;е. <span class="tex-span"><i>g</i> + <i>d</i> + <i>f</i> ≤ 1 000</span>. Все <span class="tex-span"><i>g</i> + <i>d</i> + <i>f</i></span> номеров игроков различны.</p>

## Output

<p>Выведите одно целое число&nbsp;— количество возможных стартовых составов.</p>

## Samples

```input1
1 2 3
15
10 19
20 11 13

```

```output1
1

```






```input2
2 3 4
16 40
20 12 19
13 21 11 10

```

```output2
6

```




## Note

<p>В первом примере всего один вариант для выбора состава, который удовлетворяет описанным условиям, поэтому ответ <span class="tex-span">1</span>.</p><p>Во втором примере подходят следующие игровые сочетания (в порядке вратарь-защитник-защитник-нападающий-нападающий-нападающий):</p><ul> <li> <span class="tex-font-style-tt">16 20 12 13 21 11</span> </li><li> <span class="tex-font-style-tt">16 20 12 13 11 10</span> </li><li> <span class="tex-font-style-tt">16 20 19 13 21 11</span> </li><li> <span class="tex-font-style-tt">16 20 19 13 11 10</span> </li><li> <span class="tex-font-style-tt">16 12 19 13 21 11</span> </li><li> <span class="tex-font-style-tt">16 12 19 13 11 10</span> </li></ul><p>Таким образом, ответ на этот пример — <span class="tex-span">6</span>.</p>
