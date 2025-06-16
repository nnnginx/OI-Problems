## Description

<div><p>Основой любой социальной сети является отношение дружбы между двумя пользователями в том или ином смысле. В одной известной социальной сети дружба симметрична, то есть если <span class="tex-span"><i>a</i></span> является другом <span class="tex-span"><i>b</i></span>, то <span class="tex-span"><i>b</i></span> также является другом <span class="tex-span"><i>a</i></span>. </p><p>В этой же сети есть функция, которая демонстрирует множество людей, имеющих высокую вероятность быть знакомыми для пользователя. Эта функция работает следующим образом. Зафиксируем пользователя <span class="tex-span"><i>x</i></span>. Пусть некоторый другой человек <span class="tex-span"><i>y</i></span>, не являющийся другом <span class="tex-span"><i>x</i></span> на текущий момент, является другом не менее, чем для <span class="tex-span"><i>k</i>%</span> друзей <span class="tex-span"><i>x</i></span>. Тогда он является предполагаемым другом для <span class="tex-span"><i>x</i></span>.</p><p>У каждого человека в социальной сети есть свой уникальный идентификатор — это целое число от <span class="tex-span">1</span> до <span class="tex-span">10<sup class="upper-index">9</sup></span>. Вам дан список пар пользователей, являющихся друзьями. Определите для каждого упомянутого пользователя множество его предполагаемых друзей.</p></div><div class="input-specification"><p>В первой строке следуют два целых числа <span class="tex-span"><i>m</i></span> и <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 100</span>) — количество пар друзей и необходимый процент общих друзей для того, чтобы считаться предполагаемым другом.</p><p>В последующих <span class="tex-span"><i>m</i></span> строках записано по два числа <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), обозначающих идентификаторы пользователей, являющихся друзьями. </p><p>Гарантируется, что каждая пара людей фигурирует в списке не более одного раза.</p></div><div class="output-specification"><p>Для всех упомянутых людей в порядке возрастания id выведите информацию о предполагаемых друзьях. Информация должна иметь вид "<span class="tex-span"><i>id</i>: &nbsp;<i>k</i>&nbsp;<i>id</i><sub class="lower-index">1</sub>&nbsp;<i>id</i><sub class="lower-index">2</sub>&nbsp;...&nbsp;<i>id</i><sub class="lower-index"><i>k</i></sub></span>", где <span class="tex-span"><i>id</i></span> — это id самого человека, <span class="tex-span"><i>k</i></span> — количество его предполагаемых друзей, а <span class="tex-span"><i>id</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>id</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>id</i><sub class="lower-index"><i>k</i></sub></span> — идентификаторы его предполагаемых друзей в возрастающем порядке. </p></div>


## Input

<p>В первой строке следуют два целых числа <span class="tex-span"><i>m</i></span> и <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 100</span>) — количество пар друзей и необходимый процент общих друзей для того, чтобы считаться предполагаемым другом.</p><p>В последующих <span class="tex-span"><i>m</i></span> строках записано по два числа <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>), обозначающих идентификаторы пользователей, являющихся друзьями. </p><p>Гарантируется, что каждая пара людей фигурирует в списке не более одного раза.</p>


## Output

<p>Для всех упомянутых людей в порядке возрастания id выведите информацию о предполагаемых друзьях. Информация должна иметь вид "<span class="tex-span"><i>id</i>: &nbsp;<i>k</i>&nbsp;<i>id</i><sub class="lower-index">1</sub>&nbsp;<i>id</i><sub class="lower-index">2</sub>&nbsp;...&nbsp;<i>id</i><sub class="lower-index"><i>k</i></sub></span>", где <span class="tex-span"><i>id</i></span> — это id самого человека, <span class="tex-span"><i>k</i></span> — количество его предполагаемых друзей, а <span class="tex-span"><i>id</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>id</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>id</i><sub class="lower-index"><i>k</i></sub></span> — идентификаторы его предполагаемых друзей в возрастающем порядке. </p>


## Samples

```input1
5 51
10 23
23 42
39 42
10 39
39 58

```

```output1
10: 1 42
23: 1 39
39: 1 23
42: 1 10
58: 2 10 42

```






```input2
5 100
1 2
1 3
1 4
2 3
2 4

```

```output2
1: 0
2: 0
3: 1 4
4: 1 3

```



