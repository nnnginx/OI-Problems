# AT_abc019_4 [ABC019D] 高橋くんと木の直径

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc019/tasks/abc019_4

高橋くんは木の直径を求めるのに夢中です。 木とは、頂点とそれを結ぶ辺からなる構造「グラフ」の $ 1 $ 種で、頂点の数を $ N $ 個とすると、辺は $ N-1 $ 本あり、どの頂点も他の全ての頂点に辺で間接・直接的につながっています。

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc019_4/cfb0270dd13592a982ed72200a9f86b2a95a3a4d.png)

この問題では、辺には整数の重みがついています。2頂点の間の距離を、その2つの頂点をつなぐ辺の重みの和と定義します。

木の直径とは、最も離れた2つの頂点の間の距離です。

以下のような木を考えてみましょう。辺の側に書かれた数が、その辺の重みです。

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc019_4/a33a3d0111cd3e05457375697b0a6985f92b86a4.png)

この場合、頂点 $ 1 $ と $ 2 $ の距離は $ 1 $、頂点 $ 2 $ と $ 4 $ の間の距離は $ 1+2=3 $ となります。頂点 $ 3 $ と $ 5 $ の間の距離は $ 3+4=7 $、頂点 $ 4 $ と $ 5 $ の間の距離も $ 2+1+4=7 $ で、この距離がこの木の頂点の間では最大なので、木の直径は $ 7 $ となります。

高橋くんは、頂点の数と $ 2 $ 頂点間の距離の情報から、木の直径を求めることに興味が出てきました。 この問題では、あなたは木の頂点の数 $ N $ を最初に与えられ、$ 2 $ 頂点の間の距離を尋ねる質問を何回か行い、木の直径を求めます。

ただし、$ 2 $ 頂点間の距離を聞く回数には制限があります。

制限された質問の回数以内で木の直径を求めるプログラムを書いてください。

### Input &amp; Output Format

まず，木の頂点の数 $ N $ が標準入力に与えられる。

> $ N $

続いて，あなたのプログラムは何回か応答プログラムに質問をする．質問のフォーマットは以下のとおりである。

> ? $ a $ $ b $

この質問で，$ a,b $ 間の距離が標準入力に1行で渡される。$ 1\ ≦\ a,\ b\ ≦\ N $ かつ $ a≠b $ を満たしていなければならない。

何回か質問を行った後、あなたは木の直径を当てる。木の直径を $ diameter $ とおくと、

> ! $ diameter $

というフォーマットで出力する。木の直径を出力した後、あなたのプログラムは直ちに終了しなければならない。終了しなかった場合のジャッジ結果は不定である。

また、これら以外のフォーマットで出力した場合のジャッジ結果も不定である。

この問題ではテストケースごとに質問回数の上限値が設定されており、プログラムの行った質問の回数がその上限値を上回ると誤答と判定される。

正答かどうかは木の直径の出力で判断される。木の直径を特定し得ない質問しかしていない場合でも、直径が正しければ正答となる。

- - - - - -

頂点 $ 1 $ と頂点 $ 2 $ の間の距離を質問し、$ dist $ という変数で結果を受け取る例をいくつかの言語について示す。

ただし、ここに書かれている方法以外で入出力を行っても良い。

出力した後に、出力をflushしなければならないことに注意せよ。flushしなかった場合、TLEとなることがある。

C

```
<pre class="prettyprint linenums" style="font-size: 12px; letter-spacing: 0;">
printf("? %d %d\n", 1, 2);
fflush(stdout);
scanf("%d", &dist);
```

C++

```
<pre class="prettyprint linenums" style="font-size: 12px; letter-spacing: 0;">
cout > dist;
```

Java

```
<pre class="prettyprint linenums" style="font-size: 12px; letter-spacing: 0;">
System.out.printf("? %d %d\n", 1, 2);
Scanner scanner = new Scanner(System.in);
dist = scanner.nextInt();
```

C#

```
<pre class="prettyprint linenums" style="font-size: 12px; letter-spacing: 0;">
Console.WriteLine("? {0} {1}", 1, 2);
dist = int.Parse(Console.ReadLine());
```

D

```
<pre class="prettyprint linenums" style="font-size: 12px; letter-spacing: 0;">
writeln("? ", 1, " ", 2);
stdout.flush();
dist = readln.chomp.to!int;
```

PHP

```
<pre class="prettyprint linenums" style="font-size: 12px; letter-spacing: 0;">
echo "? ", 1, " ", 2, PHP_EOL;
$ dist\ =\ trim(fgets(STDIN));


Python

print\ "?\ {0}\ {1}".format(1,\ 2)
sys.stdout.flush()
dist\ =\ int(raw_input())


Perl $|=1;
print "? ", 1, " ", 2, "\n";
$dist = ;
```

Ruby

```
<pre class="prettyprint linenums" style="font-size: 12px; letter-spacing: 0;">
print "? ", 1, " ", 2, "\n"
STDOUT.flush
dist = gets.to_i
```

## 输入格式

无

## 输出格式

无

## 说明/提示

### 制約

- $ 2\ ≦\ N\ ≦\ 50 $
- $ 1\ ≦\ (それぞれの辺の重み)\ ≦\ 10^6 $

### 部分点

この問題には部分点が設定されている。

- $ 20 $ 点分のテストケースにおいて、質問回数の上限値は 1300 回である。
- 別の $ 80 $ 点分のテストケースにおいて、質問回数の上限値は 100 回である。

### 入出力例

木が以下のような形状のとき、

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc019_4/cee5f2e74e5e3c979be3ad1dfb861be11590dd76.png)

以下のような入出力が考えられる。

 プログラムへの入力 プログラムの出力 5     ? 1 2 5     ? 2 4 1     ? 4 5 2     ? 2 3 9     ? 1 5 8     ! 14これは入出力の一つの例であり、意味のある質問をしているとは限らない。