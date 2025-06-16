## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc056/tasks/abc056_a

シカのAtCoDeerくんとTopCoDeerくんが「正直者か嘘つきか」ゲームをしています。 このゲームでは、正直者は常にほんとうのことを言い、嘘つきは常に嘘を言います。 文字 $ a $ と $ b $ が入力として与えられます。これらはそれぞれ `H` か `D` のどちらかです。

$ a $=`H` のとき、AtCoDeerくんは正直者です。 $ a $=`D` のとき、AtCoDeerくんは嘘つきです。 $ b $=`H` のとき、AtCoDeerくんは「TopCoDeerくんは正直者だ」と発言しています。 $ b $=`D` のとき、AtCoDeerくんは「TopCoDeerくんは嘘つきだ」と発言しています。

これらから判断して、TopCoDeerくんが正直者かどうか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $

## 输出格式
TopCoDeerくんが正直者なら `H` を、嘘つきなら `D` を出力せよ。

## 题目大意
题目描述：
AtcoDeer和TokadDeer在玩"正直的人或骗子"的游戏。在这个游戏中，正直的人总是说实话，骗子总是说谎。输入为两个字符串a和b,a和b均为"H"或"D"。
当a为H的时候，表明AtcoDeer是正直的人。当a为D的时候，表明AtcoDeer是个骗子。这时在b为H的时候，AtCODeer断定TokcoDeer是个正直的人，当b为D的时候,AtcoDeer断定TokcoDeer是骗子”。反之也成立。

你需要根据输入的两个字符串帮AtcoDeer断定TokadDeer是骗子还是正直的人，如果是正直的人，则输出"H"，否则输出"D"。

```input1
H H
```

```output1
H
```

```input2
D H
```

```output2
D
```

```input3
D D
```

```output3
H
```

## 提示
### 制約

- $ a $=`H` または `D`
- $ b $=`H` または `D`

### Sample Explanation 1

AtCoDeerくんは正直者なので、AtCoDeerくんの言っているとおりTopCoDeerくんは正直者です。

### Sample Explanation 2

今度はAtCoDeerくんは嘘つきなので、AtCoDeerくんの言っていることとは異なりTopCoDeerくんは嘘つきです。

