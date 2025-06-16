# AT_arc003_2 [ARC003B] さかさま辞書

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc003/tasks/arc003_2

高橋君は友達とチャットで逆さしりとりをすることにしました。  
 逆さしりとりとは、前の人が言った単語の頭文字で終わる単語を答えるしりとりです。  
 しかし、高橋君は英単語に自信がないのでこっそり「さかさま辞書」を使うことにしました。  
  
 普通の辞書は単語の先頭の文字がABC順になるように並べられており、同じ文字同士の場合はその次の文字がABC順になるように並べられます。  
 先頭から見ていく普通の辞書順に対して、「さかさま辞書」は後ろの文字から見ていきます。  
 例えば apple, bee, card は、普通の辞書なら apple → bee → card の順になります。  
 しかし、「さかさま辞書」では d で終わる card が $ 1 $ 番、apple とbee は同じ e で終わるのでその $ 1 $ つ前が e である bee が $ 2 $ 番、l であるapple が $ 3 $ 番の順になります。

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_arc003_2/3b080c0561a840fa2991f0f7f5be6d4cfe660742.png)図(a)：普通の辞書順に並べた例 図(b)：さかさま辞書順に並べた例

 

   
 高橋君の代わりに「さかさま辞書」を作成し、与えられた単語を「さかさま辞書」順に並べてください。 入力は以下の形式で標準入力から与えられる。 > $ N $ $ s_{1} $ $ s_{2} $ : : $ s_{N} $

- $ 1 $ 行目は、並べる単語数を表す整数 $ N\ (1\ ≦\ N\ ≦\ 100) $ が与えられる。
- $ 2 $ 行目から $ N $ 行は、並べる単語を表す文字列が $ 1 $ 行に $ 1 $ つずつ与えられる。
- $ i+1 $ 行目の文字列 $ s_i $ の長さは $ 1 $ 文字以上 $ 20 $ 文字以下で、含まれる文字はアルファベットの小文字のみ(`a`-`z`)です。
- なお、重複する単語が与えられることはありません。
 
 入力として与えられた単語を、さかさま辞書順に標準出力に $ 1 $ 行ずつ出力せよ。  
 なお、最後には改行を出力せよ。 ```
<pre class="prettyprint linenums">
5
chokudai
kensho
imos
yuichirw
ao
```

 ```
<pre class="prettyprint linenums">
chokudai
ao
kensho
imos
yuichirw
```

- まず、それぞれの一番後ろの文字は、chokudai、kensho、imos、yuichirw、aoなのでABC順に並べると、i,o,s,wの順になります。
- しかしkenshoとaoの $ 2 $ 人が同じ o なので、この $ 2 $ 人に関してはその $ 1 $ つ前の文字の順で並べます。
- kenshoの後ろから $ 2 $ つ目の文字は h、ao の後ろから $ 2 $ つ目の文字は a なので、ao, kensho の順になります。
- よって、chokudai, ao, kensho, imos, yuichirw の順が答えになります。
 
```
<pre class="prettyprint linenums">
2
dart
art
```

 ```
<pre class="prettyprint linenums">
art
dart
```

- 後ろから $ 1,2,3 $ 番目とも同じ文字なので、後ろから $ 4 $ 番目の文字を比較します。
- しかし、art の後ろから $ 4 $ 番目の文字はありません。
- 無い場合は、a よりも早いので、art, dart の順になります。

## 输入格式

无

## 输出格式

无