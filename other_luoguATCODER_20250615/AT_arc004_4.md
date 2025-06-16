# AT_arc004_4 [ARC004D] 表現の自由 ( Freedom of expression )

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc004/tasks/arc004_4

整数 $ N $ と $ M $ が与えられる時、整数 $ N $ を $ M $ 個の整数の積で表す方法は何通りあるでしょうか。  
 その答えを $ 1,000,000,007 $ で割った余りを答えてください。 入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

- 入力は $ 1 $ 行のみからなり、整数 $ N(1\ ≦\ |N|\ ≦\ 10^9) $ と整数 $ M(1\ ≦\ M\ ≦\ 10^5) $ が空白区切りで与えられる。
 
 整数 $ N $ を $ M $ 個の整数の積で表す方法の数を $ 1,000,000,007 $ で割った余りを標準出力に $ 1 $ 行で出力せよ 。  
 なお、最後には改行を出力せよ。 ```
<pre class="prettyprint linenums">
10 2
```

 ```
<pre class="prettyprint linenums">
8
```

- $ 10 $ を $ 2 $ つの整数の積で表す方法は以下の $ 8 $ 通りになります。
- $ 1\ \times\ 10 $
- $ 2\ \times\ 5 $
- $ 5\ \times\ 2 $
- $ 10\ \times\ 1 $
- $ (-1)\ \times\ (-10) $
- $ (-2)\ \times\ (-5) $
- $ (-5)\ \times\ (-2) $
- $ (-10)\ \times\ (-1) $
 

```
<pre class="prettyprint linenums">
1000000000 1
```

 ```
<pre class="prettyprint linenums">
1
```

- $ 1,000,000,000 $ を $ 1 $ つの積で書き表すには $ 1,000,000,000 $ と書くしか無いので、$ 1 $ 通りになります。

```
<pre class="prettyprint linenums">
-2 3
```

 ```
<pre class="prettyprint linenums">
12
```

- $ -2 $ を $ 3 $ つの整数の積で表す方法は以下の $ 12 $ 通りになります。
- $ 1\ \times\ 1\ \times\ (-2) $
- $ 1\ \times\ 2\ \times\ (-1) $
- $ 1\ \times\ (-1)\ \times\ 2 $
- $ 1\ \times\ (-2)\ \times\ 1 $
- $ 2\ \times\ 1\ \times\ (-1) $
- $ 2\ \times\ (-1)\ \times\ 1 $
- $ (-1)\ \times\ 1\ \times\ 2 $
- $ (-1)\ \times\ 2\ \times\ 1 $
- $ (-1)\ \times\ (-1)\ \times\ (-2) $
- $ (-1)\ \times\ (-2)\ \times\ (-1) $
- $ (-2)\ \times\ 1\ \times\ 1 $
- $ (-2)\ \times\ (-1)\ \times\ (-1) $
 

```
<pre class="prettyprint linenums">
50 1000
```

 ```
<pre class="prettyprint linenums">
96554651
```

## 输入格式

无

## 输出格式

无