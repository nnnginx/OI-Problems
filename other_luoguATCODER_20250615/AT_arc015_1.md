# AT_arc015_1 [ARC015A] Celsius と Fahrenheit

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc015/tasks/arc015_1

摂氏での温度 $ n $ 度を華氏にで表すと $ (\ 9\ ÷\ 5\ ×\ n\ )\ +\ 32 $ 度となります。  
 摂氏での温度が与えられるので華氏での温度に変換するプログラムを書いてください。  
 入力は以下の形式で標準入力から与えられる。

> $ n $

- $ 1 $ 行目は、華氏に変換すべき、摂氏の温度 $ n\ (-273≦n≦1,000) $ が整数で与えられる。
 
 摂氏での温度 $ n $ を華氏に変換し、その値を $ 1 $ 行で出力せよ。  
 なお、出力の最後には改行をいれること。  
 出力は絶対誤差あるいは相対誤差の少なくとも片方が $ 10^{-6} $ 以下であれば許容される。 ```
<pre class="prettyprint linenums">
10
```

 ```
<pre class="prettyprint linenums">
50
```

- $ (9÷5×10)+32 $ $ = $ $ 50 $
 
```
<pre class="prettyprint linenums">
33
```

 ```
<pre class="prettyprint linenums">
91.4
```

- $ (9÷5×33)+32 $ $ = $ $ 91.4 $
- 摂氏での温度が整数であっても、華氏での温度は整数になるとは限りません。
 
```
<pre class="prettyprint linenums">
-100
```

 ```
<pre class="prettyprint linenums">
-148
```

- $ 9÷5×(-100) $ $ +32 $ $ = $ $ -148 $

## 输入格式

无

## 输出格式

无