# AT_colopl2018_final_b 異世界数式

## 题目描述

[problemUrl]: https://atcoder.jp/contests/colopl2018-final/tasks/colopl2018_final_b

あなたは異世界で店舗経営をするシミュレーションゲームで遊んでいます。この異世界では、四則演算を含む数式の表現方法が通常のものと異なるようです。

ふつう数式を書くときは、四則演算は演算子を中置する `1+2+3` や `10/5` といった形で表しますが、この世界では四則演算を関数呼出しのような形で表します。たとえば、さきほどの例に対応する数式は `+(1,2,3)` や `/(10,5)` となります。

より厳密に言うとこの世界での数式は、単なる数字の列か、もしくは演算子 (`+`, `-`, `*`, `/` のいずれか) の直後で括弧 (`(`) を開き、その中に数式をいくつかカンマ (`,`) で区切って並べ、その後括弧 (`)`) を閉じるという形式で表されます。ここで、括弧の中に現れる数式の個数は、加算と乗算 (`+`, `*`) のときは $ 1 $ つ以上ならいくつでも構いませんが、減算と除算 (`-`, `/`) のときは必ず $ 2 $ 個です。

たとえば、`0123` や `+(10,*(20,30),-(40,50))` や `*(5)` はいずれも正しい数式です。いっぽう、`+((1))` や `-(5)` といった文字列は正しい数式ではありません。

異世界の数式を表す文字列 $ S $ が与えられたとき、それを通常の (中置記法の) 数式に変換するプログラムを作成してください。ただし、変換後の数式は以下の条件を満たす必要があります。

- 変換後の数式における括弧は、変換前の括弧と対応する箇所にだけちょうど現れる必要があります。たとえば、`+(1,-(2,3))` は `(1+(2-3))` と変換し、`*(5)` は `(5)` と変換しなければなりません。
- 入力中に現れる数は先頭の `0` なども含めてそのまま出力せねばなりません。
- 余計な空白を入れてはいけません。たとえば、`+(1,2)` を `(1 + 2)` のように変換してはならず、`(1+2)` とする必要があります。

これらの条件について、より詳細には入出力例も参照してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

変換後の数式を $ 1 $ 行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
*(*(0,5),+(14,3),-(5,77))
```

### 输出 #1

```
((0*5)*(14+3)*(5-77))
```

## 输入输出样例 #2

### 输入 #2

```
+(1,+(+(2,3)),+(4,+(5)))
```

### 输出 #2

```
(1+((2+3))+(4+(5)))
```

## 输入输出样例 #3

### 输入 #3

```
9876
```

### 输出 #3

```
9876
```

## 输入输出样例 #4

### 输入 #4

```
+(123456789,12345678901234567890,0,00,000,0123456789)
```

### 输出 #4

```
(123456789+12345678901234567890+0+00+000+0123456789)
```

## 输入输出样例 #5

### 输入 #5

```
*(5)
```

### 输出 #5

```
(5)
```

## 说明/提示

### 制約

- $ 1\ \leq\ |S|\ \leq\ 10^5 $
- 文字列 $ S $ は演算子 (`+`, `-`, `*`, `/`)、括弧 (`(`, `)`)、カンマ (`,`)、数字のみからなる、異世界の数式として正しい文字列である。

### Sample Explanation 2

括弧の位置と個数に十分注意してください。

### Sample Explanation 4

数式中に現れる数に明示的な上限はありません。また、数を表記する際に、先頭が `0` であるような表記法も正しいとされていること、およびそのように表記された数はそのまま出力せねばならないことにも注意してください。