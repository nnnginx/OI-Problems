## Description

<div><p>Немногие знают, что сотрудники ВКонтакте могут менять цвет подсветки в куполе знаменитого Дома Зингера, где расположена штаб-квартира ВКонтакте. Для этого нужно всего лишь отправить сообщение с цветом в специальный чат «Зингер | color», а бот его распознает и сменит подсветку. При этом на время городских мероприятий смена цвета блокируется.</p><p>Формально, бот обрабатывает три типа сообщений: </p><ul> <li> <span class="tex-font-style-tt">lock</span>: заблокировать изменение цвета. Если оно и так заблокировано на данный момент, сообщение игнорируется. </li><li> <span class="tex-font-style-tt">unlock</span>: разблокировать изменение цвета. Если оно и так разблокировано на данный момент, сообщение игнорируется. </li><li> <span class="tex-font-style-tt">red</span> / <span class="tex-font-style-tt">orange</span> / <span class="tex-font-style-tt">yellow</span> / <span class="tex-font-style-tt">green</span> / <span class="tex-font-style-tt">blue</span> / <span class="tex-font-style-tt">indigo</span> / <span class="tex-font-style-tt">violet</span>: изменить цвет купола на заданный, если изменение цвета на данный момент не заблокировано. </li></ul><p>Вам дана история сообщений, полученных ботом, в хронологическом порядке. Считайте, что перед получением первого сообщения купол подсвечивается голубым (<span class="tex-font-style-tt">blue</span>), а изменение цвета не заблокировано.</p><p>В качестве эксперимента было решено поддержать в боте эффективную обработку редактирования сообщений. Вам дана последовательность пар вида $(i, msg)$, означающих, что $i$-е в хронологическом порядке сообщение было отредактировано и теперь имеет вид $msg$. Обратите внимание, что редактироваться может любое сообщение, и при редактировании сообщения бот должен обработать всю историю сообщений заново (в частности, перед обработкой первого сообщения цвет купола голубой, а изменение цвета не заблокировано).</p><p>Определите, какой цвет будет у купола Дома Зингера до первой операции редактирования, а также после каждой операции редактирования.</p></div><div class="input-specification"><p>В первой строке задано одно целое число $n$ ($1 \le n \le 10^5$)&nbsp;— число сообщений, полученных ботом.</p><p>В следующих $n$ строках заданы сообщения, полученные ботом, в хронологическом порядке, по одному сообщению в строке. Каждое сообщение&nbsp;— строка из следующего набора: <span class="tex-font-style-tt">lock</span>, <span class="tex-font-style-tt">unlock</span>, <span class="tex-font-style-tt">red</span>, <span class="tex-font-style-tt">orange</span>, <span class="tex-font-style-tt">yellow</span>, <span class="tex-font-style-tt">green</span>, <span class="tex-font-style-tt">blue</span>, <span class="tex-font-style-tt">indigo</span>, <span class="tex-font-style-tt">violet</span>. Сообщения пронумерованы от $1$ до $n$.</p><p>В следующей строке задано одно целое число $t$ ($1 \le t \le 10^5$)&nbsp;— число операций редактирования сообщений.</p><p>В следующих $t$ строках заданы операции редактирования в хронологическом порядке, по одной в строке. Каждая операция&nbsp;— пара из номера сообщения $i$ ($1 \le i \le n$) и его нового содержимого $msg$, также принадлежащего набору <span class="tex-font-style-tt">lock</span>, <span class="tex-font-style-tt">unlock</span>, <span class="tex-font-style-tt">red</span>, <span class="tex-font-style-tt">orange</span>, <span class="tex-font-style-tt">yellow</span>, <span class="tex-font-style-tt">green</span>, <span class="tex-font-style-tt">blue</span>, <span class="tex-font-style-tt">indigo</span>, <span class="tex-font-style-tt">violet</span>.</p></div><div class="output-specification"><p>Выведите $t+1$ строку: цвет купола до первой операции редактирования, а также после каждой операции редактирования в хронологическом порядке.</p></div>

## Input

<p>В первой строке задано одно целое число $n$ ($1 \le n \le 10^5$)&nbsp;— число сообщений, полученных ботом.</p><p>В следующих $n$ строках заданы сообщения, полученные ботом, в хронологическом порядке, по одному сообщению в строке. Каждое сообщение&nbsp;— строка из следующего набора: <span class="tex-font-style-tt">lock</span>, <span class="tex-font-style-tt">unlock</span>, <span class="tex-font-style-tt">red</span>, <span class="tex-font-style-tt">orange</span>, <span class="tex-font-style-tt">yellow</span>, <span class="tex-font-style-tt">green</span>, <span class="tex-font-style-tt">blue</span>, <span class="tex-font-style-tt">indigo</span>, <span class="tex-font-style-tt">violet</span>. Сообщения пронумерованы от $1$ до $n$.</p><p>В следующей строке задано одно целое число $t$ ($1 \le t \le 10^5$)&nbsp;— число операций редактирования сообщений.</p><p>В следующих $t$ строках заданы операции редактирования в хронологическом порядке, по одной в строке. Каждая операция&nbsp;— пара из номера сообщения $i$ ($1 \le i \le n$) и его нового содержимого $msg$, также принадлежащего набору <span class="tex-font-style-tt">lock</span>, <span class="tex-font-style-tt">unlock</span>, <span class="tex-font-style-tt">red</span>, <span class="tex-font-style-tt">orange</span>, <span class="tex-font-style-tt">yellow</span>, <span class="tex-font-style-tt">green</span>, <span class="tex-font-style-tt">blue</span>, <span class="tex-font-style-tt">indigo</span>, <span class="tex-font-style-tt">violet</span>.</p>

## Output

<p>Выведите $t+1$ строку: цвет купола до первой операции редактирования, а также после каждой операции редактирования в хронологическом порядке.</p>

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
6
5 green
6 lock
6 yellow
4 lock
1 lock
5 unlock
```

```output1
orange
green
green
indigo
violet
blue
indigo
```






```input2
1
red
8
1 lock
1 unlock
1 blue
1 unlock
1 unlock
1 lock
1 yellow
1 lock
```

```output2
red
blue
blue
blue
blue
blue
blue
yellow
blue
```



