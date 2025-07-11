# AT_abc332_c [ABC332C] T-shirts

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc332/tasks/abc332_c

AtCoder 社は[ロゴ入りの T シャツ](https://suzuri.jp/AtCoder/5510290/t-shirt/s/ash)を販売しています。

高橋君の $ N $ 日間の予定が `0`, `1`, `2` のみからなる長さ $ N $ の文字列 $ S $ で与えられます。  
具体的には、$ 1\leq\ i\leq\ N $ をみたす整数 $ i $ について、

- $ S $ の $ i $ 文字目が `0` のとき、$ i $ 日目に何の予定も入っていません。
- $ S $ の $ i $ 文字目が `1` のとき、$ i $ 日目に高橋君は食事に行く予定があります。
- $ S $ の $ i $ 文字目が `2` のとき、$ i $ 日目に高橋君は競技プログラミングのイベントに行く予定が入っています。

高橋君は無地の T シャツを $ M $ 枚持っており、$ 1 $ 日目の直前の時点ですべて洗濯済みの状態となっています。  
これに加えて、次の条件をみたすように行動できるように、高橋君は AtCoder のロゴ入りの T シャツを何枚か購入する事にしました。

- 食事に行く日には、無地の T シャツ $ 1 $ 枚またはロゴ入りの T シャツ $ 1 $ 枚を着用する。
- 競技プログラミングのイベントに行く日にはロゴ入りの T シャツ $ 1 $ 枚を着用する。
- 何の予定もない日には T シャツを着用しない。加えて、その時点で着用済みの T シャツを全て洗濯する。 洗濯した T シャツは翌日から着用できる。
- 一度着用した T シャツは次に洗濯するまで着用できない。

$ N $ 日間のうち予定が入っている日すべてについて、条件をみたす T シャツを着用できるようにするために、高橋君は最低何枚のTシャツを購入する必要があるか求めてください。 新しく T シャツを購入する必要がないならば $ 0 $ を出力してください。  
ただし、購入した T シャツも $ 1 $ 日目の直前の時点ですべて洗濯済みの状態で存在するものとします。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ S $

## 输出格式

問題文の条件をみたすように行動するために 高橋君が購入する必要のある $ T $ シャツの枚数の最小値を出力せよ。  
新しく購入する必要がないならば $ 0 $ を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
6 1
112022
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
3 1
222
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
2 1
01
```

### 输出 #3

```
0
```

## 说明/提示

### 制約

- $ 1\leq\ M\leq\ N\leq\ 1000 $
- $ S $ は `0`, `1`, `2` のみからなる長さ $ N $ の文字列
- $ N,M $ は整数

### Sample Explanation 1

高橋君がロゴ入りの T シャツを $ 2 $ 枚購入したとき、次のようにして高橋君は T シャツを着用することができます。 - $ 1 $ 日目、高橋君はロゴ入りの T シャツを着用して食事に行きます。 - $ 2 $ 日目、高橋君は無地の T シャツを着用して食事に行きます。 - $ 3 $ 日目、高橋君はロゴ入りの T シャツを着用して競技プログラミングのイベントに行きます。 - $ 4 $ 日目、高橋君は予定がないため、着用した T シャツをすべて洗濯します。これにより、$ 1,2,3 $ 日目に着用した T シャツを再び着用することが可能になります。 - $ 5 $ 日目、高橋君はロゴ入りの T シャツを着用して競技プログラミングのイベントに行きます。 - $ 6 $ 日目、高橋君はロゴ入りの T シャツを着用して競技プログラミングのイベントに行きます。 高橋君がロゴ入りの T シャツを $ 1 $ 枚以下しか購入しなかった場合には、 どのようにしても条件をみたすように T シャツを着用することができません。 よって、$ 2 $ を出力します。

### Sample Explanation 3

高橋君は新しく T シャツを購入する必要はありません。