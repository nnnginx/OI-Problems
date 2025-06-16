## Description

<div><p>Прошло много лет, и на вечеринке снова встретились <span class="tex-span"><i>n</i></span> друзей. С момента последней встречи техника шагнула далеко вперёд, появились фотоаппараты с автоспуском, и теперь не требуется, чтобы один из друзей стоял с фотоаппаратом, и, тем самым, оказывался не запечатлённым на снимке.</p><p>Упрощенно процесс фотографирования можно описать следующим образом. На фотографии каждый из друзей занимает прямоугольник из пикселей: в стоячем положении <span class="tex-span"><i>i</i></span>-й из них занимает прямоугольник ширины <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> пикселей и высоты <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> пикселей. Но также, при фотографировании каждый человек может лечь, и тогда он будет занимать прямоугольник ширины <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> пикселей и высоты <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> пикселей.</p><p>Общая фотография будет иметь размеры <span class="tex-span"><i>W</i> × <i>H</i></span>, где <span class="tex-span"><i>W</i></span> — суммарная ширина всех прямоугольников-людей, а <span class="tex-span"><i>H</i></span> — максимальная из высот. Друзья хотят определить, какую минимальную площадь может иметь общая фотография. Помогите им в этом.</p></div><div class="input-specification"><p>В первой строке следует целое число <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — количество друзей.</p><p>В последующих <span class="tex-span"><i>n</i></span> строках следуют по два целых числа <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), обозначающие размеры прямоугольника, соответствующего <span class="tex-span"><i>i</i></span>-му из друзей.</p></div><div class="output-specification"><p>Выведите единственное целое число, равное минимальной возможной площади фотографии, вмещающей всех друзей.</p></div>


## Input

<p>В первой строке следует целое число <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — количество друзей.</p><p>В последующих <span class="tex-span"><i>n</i></span> строках следуют по два целых числа <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), обозначающие размеры прямоугольника, соответствующего <span class="tex-span"><i>i</i></span>-му из друзей.</p>


## Output

<p>Выведите единственное целое число, равное минимальной возможной площади фотографии, вмещающей всех друзей.</p>


## Samples

```input1
3
10 1
20 2
30 3

```

```output1
180

```






```input2
3
3 1
2 2
4 3

```

```output2
21

```






```input3
1
5 10

```

```output3
50

```



