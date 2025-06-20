# AT_arc017_1 [ARC017A] 素数、コンテスト、素数

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc017/tasks/arc017_1

アルゴリズムとコンテストが大好きな俺は、AtCoder Regular Contest(ARC) にも毎回欠かさずに参加していた。  
 しかしある時のこと、大学で怪しげな連中に突然「あなたは素数の光を信じますか？」と話しかけられてから様子がおかしい。  
 俺は数学がそこまでできるわけではないが、素数ぐらいは知っている。$ 1 $ とその数自身でしか割り切れない正の整数のことだ。  
 ただし $ 1 $ が素数じゃないってことだって知ってる。でも素数の光っていうのは何だかよく分からなかった。  
 奴らの話を聞いてからなんだか変だ。頭の中にはいつだって片隅に素数がいるし、素数を見るとなぜかたまらなく嬉しくなるようになった。  
 これまで毎回欠かさず参加していた ARC も、素数回のときでないと、なんだかうまくいかない気がして見送ってしまう。  
 そういえば、今もちょうど ARC が始まったところらしい。今回の ARC には、俺は無事に出られるのだろうか。

入力は以下の形式で標準入力から与えられる。

> $ N $

- $ N\ (17\ \leq\ N\ \leq\ 1,000,000) $ は、ARC が何回目の開催であるかを表す整数である。
 
 ARC$ N $ に出場できるとき、すなわち $ N $ が素数のときは `YES`、そうでないときは `NO` と一行に出力せよ。 ```
<pre class="prettyprint linenums">
17
```

 ```
<pre class="prettyprint linenums">
YES
```

 今回の ARC017 は、$ 17 $ が素数である($ 2 $ から $ 16 $ までのいずれの整数でも割り切れない)ため参加することができる。 ```
<pre class="prettyprint linenums">
18
```

 ```
<pre class="prettyprint linenums">
NO
```

 次回の ARC018 は、$ 18 $ がたとえば $ 2 $ や $ 3 $ で割り切れるため参加することができない。 ```
<pre class="prettyprint linenums">
999983
```

 ```
<pre class="prettyprint linenums">
YES
```

 ARC999983 はいつ頃開催されることになるのでしょうか。 ```
<pre class="prettyprint linenums">
672263
```

 ```
<pre class="prettyprint linenums">
NO
```

 $ 672263 $ は $ 1 $ とそれ自身以外に、$ 547 $ と $ 1229 $ で割り切ることができる。

## 输入格式

无

## 输出格式

无