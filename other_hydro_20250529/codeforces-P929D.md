## Description

<div><p>Герой Аркадий находится на узкой полоске земли, разделенной на <span class="tex-span"><i>n</i></span> зон, пронумерованных от <span class="tex-span">1</span> до <span class="tex-span"><i>n</i></span>. Из <span class="tex-span"><i>i</i></span>-й зоны можно пройти лишь в <span class="tex-span">(<i>i</i> - 1)</span>-ю зону и в <span class="tex-span">(<i>i</i> + 1)</span>-ю зону, если они существуют. При этом между каждой парой соседних зон находятся пограничные врата, которые могут быть разных цветов, цвет врат между <span class="tex-span"><i>i</i></span>-й и <span class="tex-span">(<i>i</i> + 1)</span>-й зоной равен <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Аркадий может пройти пограничные врата некоторого цвета, только если он перед этим побывал в одном из шатров хранителей ключей этого цвета и взял ключ. В каждой зоне находится ровно один шатер хранителя ключей некоторого цвета, цвет шатра в <span class="tex-span"><i>i</i></span>-й зоне равен <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>. После посещения шатра определенного цвета Аркадий может неограниченное число раз проходить через любые врата этого цвета.</p><p>На проход через одни врата Аркадий тратит один ход, на посещение шатра и другие перемещения ходы не требуются. За какое минимальное число ходов Аркадий может попасть из зоны <span class="tex-span"><i>a</i></span> в зону <span class="tex-span"><i>b</i></span>, если изначально у него нет никаких ключей?</p></div><div class="input-specification"><p>Первая строка содержит три целых числа <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>)&nbsp;— число зон, номер начальной зоны и номер конечной зоны, соответственно.</p><p>Вторая строка содержит <span class="tex-span"><i>n</i> - 1</span> целое число <span class="tex-span"><i>g</i><sub class="lower-index">1</sub>, <i>g</i><sub class="lower-index">2</sub>, ..., <i>g</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), где <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> означает цвет пограничных врат между зонами <span class="tex-span"><i>i</i></span> и <span class="tex-span"><i>i</i> + 1</span>.</p><p>Третья строка содержит <span class="tex-span"><i>n</i></span> целых чисел <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), где <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> означает цвет шатра хранителя ключей в <span class="tex-span"><i>i</i></span>-й зоне.</p></div><div class="output-specification"><p>Если Аркадий не может попасть из зоны <span class="tex-span"><i>a</i></span> в зону <span class="tex-span"><i>b</i></span>, не имея изначально ключей, выведите <span class="tex-font-style-tt">-1</span>.</p><p>Иначе выведите минимальное количество ходов, которое потребуется Аркадию.</p></div>

## Input

<p>Первая строка содержит три целых числа <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>)&nbsp;— число зон, номер начальной зоны и номер конечной зоны, соответственно.</p><p>Вторая строка содержит <span class="tex-span"><i>n</i> - 1</span> целое число <span class="tex-span"><i>g</i><sub class="lower-index">1</sub>, <i>g</i><sub class="lower-index">2</sub>, ..., <i>g</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), где <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> означает цвет пограничных врат между зонами <span class="tex-span"><i>i</i></span> и <span class="tex-span"><i>i</i> + 1</span>.</p><p>Третья строка содержит <span class="tex-span"><i>n</i></span> целых чисел <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), где <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> означает цвет шатра хранителя ключей в <span class="tex-span"><i>i</i></span>-й зоне.</p>

## Output

<p>Если Аркадий не может попасть из зоны <span class="tex-span"><i>a</i></span> в зону <span class="tex-span"><i>b</i></span>, не имея изначально ключей, выведите <span class="tex-font-style-tt">-1</span>.</p><p>Иначе выведите минимальное количество ходов, которое потребуется Аркадию.</p>

## Samples

```input1
5 4 1
3 1 1 2
7 1 2 1 3

```

```output1
7

```






```input2
5 1 5
4 3 2 1
4 3 2 5 5

```

```output2
-1

```




## Note

<p>В первом примере, чтобы попасть из зоны <span class="tex-span">4</span> в зону <span class="tex-span">1</span>, Аркадию нужно сначала взять ключ цвета <span class="tex-span">1</span>, пройти в зону <span class="tex-span">3</span>, там взять ключ цвета <span class="tex-span">2</span> и пройти обратно в зону <span class="tex-span">4</span> и затем в зону <span class="tex-span">5</span>, взять там ключ цвета <span class="tex-span">3</span> и дойти до зоны <span class="tex-span">1</span> за четыре хода.</p><p>Во втором примере Аркадий может дойти лишь до четвертой зоны, так как шатров хранителей ключей цвета <span class="tex-span">1</span> нет совсем.</p>
