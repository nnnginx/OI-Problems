# AT_hbpc_2 01:01

## 题目描述

[problemUrl]: https://atcoder.jp/contests/hbpc2012/tasks/hbpc_2

6月10日はhasiの誕生日なので日付問題を出します。  
 嘘です。時刻問題を出します。  
 プログラミングコンテストは世界中で開催されていますが、そこで問題になってくるのはタイムゾーンです。  
 webページには開始時間が現地時間で載っていていちいち計算しないといけません。  
 そこでhasiは、世界共通で使える、時間に付ける名前があったら便利じゃないかなと思いました。   
 10日(Sun)、11日(Mon)のような曜日のように、例えば、3時(Sun)、4時(Mon)というように名前を付けられないか、と。  
 そして、この「時間に付ける名前」を曜時と名付けました。  
 この問題は、曜時を計算する問題です。 入力は以下の形式に従う。

> $ city_A $ $ hour_0 $ $ hour_1 $ $ … $ $ hour_{23} $ $ N $ $ city_{1,1} $ $ time_{1,1} $ $ city_{1,2} $ $ time_{1,2} $ $ city_{2,1} $ $ time_{2,1} $ $ city_{2,2} $ $ time_{2,2} $ : $ city_{N,1} $ $ time_{N,1} $ $ city_{N,2} $ $ time_{N,2} $ $ city_B $ $ time_B $

 $ city_A $, $ city_B $ は、それぞれ都市 $ A $、都市 $ B $ の名前を表す。  
 $ hour_i $ は、時間の名前を表す。 都市 $ A $ において、 00:00 ～ 00:59 には $ hour_0 $、 01:00 ～ 01:59 には $ hour_1 $、 …、 23:00 ～ 23:59 には $ hour_{23} $、 という名前が与えられる。 時間の名前は世界共通であり、ある時刻において、ある都市の時間の名前が $ hour_i $ のとき、すべての都市で時間の名前が $ hour_i $ となる。  
 $ city_{i,j} $ は都市の名前、$ time_{i,j} $ は時刻を表す。 都市 $ city_{i,1} $ が時刻 $ time_{i,1} $ のとき、都市 $ city_{i,2} $ は時刻 $ time_{i,2} $ であるという情報が $ N $ 個与えられる。 - $ 1≦N≦20 $
- 都市の名前・時間の名前は大文字・小文字の英字からなる
- 都市の名前・時間の名前の文字列長は $ 20 $ 以下
- 異なる都市が同じ名前を持つことはない
- 時間の名前は互いに異なる
- 時刻は`hh:mm`の形式で与えられる
- `hh`は`00`～`23`
- `mm`は`00`～`59`
- 情報の矛盾や不足は存在しないことが保証される
 
 都市 $ B $ が時刻 $ time_B $ のときの時間の名前を求めよ。夏時間はないものとする。 ```
<pre class="prettyprint linenums">
UTC
A B C D E F G H I J K L M N O P Q R S T U V W X
1
UTC 00:00 Akashi 09:00
Akashi
00:00
```

 ```
<pre class="prettyprint linenums">
P
```

 ```
<pre class="prettyprint linenums">
Tokyo
P Q R S T U V W X A B C D E F G H I J K L M N O
3
Tokyo 00:00 Connecticut 11:00
Moskow 19:30 Connecticut 11:30
India 21:30 Moskow 20:00
India
00:39
```

 ```
<pre class="prettyprint linenums">
T
```

## 输入格式

无

## 输出格式

无