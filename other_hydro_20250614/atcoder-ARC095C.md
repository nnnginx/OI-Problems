## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc095/tasks/arc095_c

$ H $ 行 $ W $ 列のマス目があり，各マスには英小文字が書かれています． 具体的には，上から $ i $ 行，左から $ j $ 列目のマスに書かれている文字は，文字列 $ S_i $ の $ j $ 文字目に等しいです．

すぬけ君は，このマス目に対して次の操作を好きな回数行うことができます：

- $ 2 $ つの異なる行を選び，入れ替える．または，$ 2 $ つの異なる列を選び，入れ替える．

すぬけ君は，このマス目が点対称的になるようにしたいです． すなわち，任意の $ 1\ \leq\ i\ \leq\ H $, $ 1\ \leq\ j\ \leq\ W $ に対して，マス目の上から $ i $ 行，左から $ j $ 列目に書かれている文字と，マス目の上から $ H\ +\ 1\ -\ i $ 行，左から $ W\ +\ 1\ -\ j $ 列目に書かれている文字が等しくなるようにしたいです．

すぬけくんがこの目標を達成することが可能かどうか判定してください．

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ S_1 $ $ S_2 $ $ : $ $ S_H $

## 输出格式
マス目を点対称的にできるなら `YES` を，できないなら `NO` を出力せよ．

## 题目大意
给定一个包含小写字母的矩阵，每次可以整体交换两行或两列，求是否可以将其变成一个中心对称的矩阵。

```input1
2 3
arc
rac
```

```output1
YES
```

```input2
3 7
atcoder
regular
contest
```

```output2
NO
```

```input3
12 12
bimonigaloaf
faurwlkbleht
dexwimqxzxbb
lxdgyoifcxid
ydxiliocfdgx
nfoabgilamoi
ibxbdqmzxxwe
pqirylfrcrnf
wtehfkllbura
yfrnpflcrirq
wvcclwgiubrk
lkbrwgwuiccv
```

```output3
YES
```

## 提示
### 制約

- $ 1\ \leq\ H\ \leq\ 12 $
- $ 1\ \leq\ W\ \leq\ 12 $
- $ |S_i|\ =\ W $
- $ S_i $ は英小文字のみからなる

### Sample Explanation 1

下の画像に示すように，左から $ 2 $ 列目と $ 3 $ 列目を入れ替えると，マス目が点対称的になります． !\[\](https://img.atcoder.jp/arc095/2b61caf45e7c5c7311e3944f3418b0bb.png)

