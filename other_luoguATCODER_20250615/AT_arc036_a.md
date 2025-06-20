# AT_arc036_a [ARC036A] ぐっすり

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc036/tasks/arc036_a

高橋くんはこれから $ N $ 日間の睡眠の予定を建てることにしました。 $ i $ 日目には $ t_i $ 分だけ寝る予定です。

また、高橋くんは連続した $ 3 $ 日間の睡眠時間の合計が $ K $ 分を下回ると、その連続した3日目に睡眠不足になります。 厳密に言うと、 $ x≧3 $ のとき $ x-2 $ 日目、 $ x-1 $ 日目、 $ x $ 日目の睡眠時間の合計が $ K $ を下回ると、 $ x $ 日目に睡眠不足になります。 合計がちょうど $ K $になった場合は睡眠不足になりません。

あらかじめ高橋くんの睡眠の予定を与えるので、高橋くんが睡眠不足になるかどうかを求めてください。 もし睡眠不足になるならば、何日目に睡眠不足になるか求めてください。 答えが複数通り考えられるならば、最初に睡眠不足になる日を求めてください。

高橋くんは $ 1 $ 日目と $ 2 $ 日目には睡眠不足にならないものとします。 また、高橋くんは昼寝しかしないので、睡眠により日をまたぐことは考えなくて良いです。

## 输入格式

入力は以下の形式で標準入力から与えられる

> $ N $ $ K $ $ t_1 $ $ t_2 $ : $ t_N $

- $ 1 $ 行目には高橋くんが予定を建てた日数 $ N(3\ ≦\ N\ ≦\ 10^5) $ と睡眠不足の基準を表す整数 $ K(0\ ≦\ K\ ≦\ 4,320) $ が空白区切りで与えられる。
- $ 2 $ 行目からの $ N $ 行のうち $ i $ 行目には $ i $ 日目に予定している睡眠時間を表す整数 $ t_i(0\ ≦\ t_i\ ≦\ 1,440) $ が与えられる。

## 输出格式

もし高橋くんが$ N $日の間に睡眠不足にならないならば $ -1 $ を $ 1 $ 行に出力せよ。 もしなるならば、最初になる日を $ 1 $ 行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 1080
300
420
420
180
360
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
5 180
60
60
60
60
60
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
5 4230
360
360
360
360
360
```

### 输出 #3

```
3
```

## 说明/提示

### Sample Explanation 1

$ 2,\ 3,\ 4 $ 日目の睡眠時間の合計は $ 1020 $ 分となっており $ K $ を下回っています。 この日以前に睡眠不足になっている日はありません。 よって高橋くんは $ 4 $ 日目に初めて睡眠不足になります。

### Sample Explanation 2

$ 3 $ 日間の睡眠時間の合計がちょうど $ K $ の場合は睡眠不足にならないことに注意してください。