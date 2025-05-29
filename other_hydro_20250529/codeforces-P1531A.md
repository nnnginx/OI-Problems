## Description

<div><p>Немногие знают, что сотрудники ВКонтакте могут менять цвет подсветки в куполе знаменитого Дома Зингера, где расположена штаб-квартира ВКонтакте. Для этого нужно всего лишь отправить сообщение с цветом в специальный чат «Зингер | color», а бот его распознает и сменит подсветку. При этом на время городских мероприятий смена цвета блокируется.</p><p>Формально, бот обрабатывает три типа сообщений: </p><ul> <li> <span class="tex-font-style-tt">lock</span>: заблокировать изменение цвета. Если оно и так заблокировано на данный момент, сообщение игнорируется. </li><li> <span class="tex-font-style-tt">unlock</span>: разблокировать изменение цвета. Если оно и так разблокировано на данный момент, сообщение игнорируется. </li><li> <span class="tex-font-style-tt">red</span> / <span class="tex-font-style-tt">orange</span> / <span class="tex-font-style-tt">yellow</span> / <span class="tex-font-style-tt">green</span> / <span class="tex-font-style-tt">blue</span> / <span class="tex-font-style-tt">indigo</span> / <span class="tex-font-style-tt">violet</span>: изменить цвет купола на заданный, если изменение цвета на данный момент не заблокировано. </li></ul><p>Вам дана история сообщений, полученных ботом, в хронологическом порядке. Считайте, что перед получением первого сообщения купол подсвечивается голубым (<span class="tex-font-style-tt">blue</span>), а изменение цвета не заблокировано.</p><p>Определите, какой цвет будет у купола Дома Зингера после обработки этих сообщений.</p></div><div class="input-specification"><p>В первой строке задано одно целое число $n$ ($1 \le n \le 100$)&nbsp;— число сообщений, полученных ботом.</p><p>В следующих $n$ строках заданы сообщения, полученные ботом, в хронологическом порядке, по одному сообщению в строке. Каждое сообщение&nbsp;— строка из следующего набора: <span class="tex-font-style-tt">lock</span>, <span class="tex-font-style-tt">unlock</span>, <span class="tex-font-style-tt">red</span>, <span class="tex-font-style-tt">orange</span>, <span class="tex-font-style-tt">yellow</span>, <span class="tex-font-style-tt">green</span>, <span class="tex-font-style-tt">blue</span>, <span class="tex-font-style-tt">indigo</span>, <span class="tex-font-style-tt">violet</span>.</p></div><div class="output-specification"><p>Выведите цвет купола после обработки сообщений ботом.</p></div>

## Input

<p>В первой строке задано одно целое число $n$ ($1 \le n \le 100$)&nbsp;— число сообщений, полученных ботом.</p><p>В следующих $n$ строках заданы сообщения, полученные ботом, в хронологическом порядке, по одному сообщению в строке. Каждое сообщение&nbsp;— строка из следующего набора: <span class="tex-font-style-tt">lock</span>, <span class="tex-font-style-tt">unlock</span>, <span class="tex-font-style-tt">red</span>, <span class="tex-font-style-tt">orange</span>, <span class="tex-font-style-tt">yellow</span>, <span class="tex-font-style-tt">green</span>, <span class="tex-font-style-tt">blue</span>, <span class="tex-font-style-tt">indigo</span>, <span class="tex-font-style-tt">violet</span>.</p>

## Output

<p>Выведите цвет купола после обработки сообщений ботом.</p>

## Samples

```input1
7
red
violet
unlock
red
orange
lock
indigo
```

```output1
orange
```






```input2
5
lock
unlock
lock
unlock
unlock
```

```output2
blue
```



