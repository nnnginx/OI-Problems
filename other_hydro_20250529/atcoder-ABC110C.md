## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc110/tasks/abc110_c

哂弌猟忖のみからなる猟忖双 $ S $, $ T $ が嚥えられます。

猟忖双 $ S $ に��して、肝の荷恬を採業でも佩うことができます。

荷恬: 2つの��なる哂弌猟忖 $ c_1 $, $ c_2 $ を�xび、$ S $ に根まれる畠ての $ c_1 $ を $ c_2 $ に、$ c_2 $ を $ c_1 $ に崔き�Qえる

$ 0 $ 指參貧荷恬を佩って、$ S $ を $ T $ に匯崑させられるか登協してください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ S $ $ T $

## 補竃鯉塀
$ S $ を $ T $ に匯崑させられる��栽は `Yes`、そうでない��栽は `No` を竃薦せよ。

## 籾朕寄吭
艇氏誼欺喇弌亟哂猟忖銚怏撹議忖憲堪 $S$ 才 $T$。

艇辛參壓 $S$ 貧謹肝峇佩參和荷恬��

荷恬�済《饒集�音揖議弌亟哂猟忖銚 $c_1$ 才 $c_2$��隼朔繍耽肝竃�峙� $c_1$ 紋算葎 $c_2$��旺繍耽肝竃�峙� $c_2$ 紋算葎 $c_1$。

宥狛峇佩巣肝賜厚謹肝荷恬��鳩協 $S$ 才 $T$ 頁倦辛參�犁函�

```input1
azzel
apple
```

```output1
Yes
```

```input2
chokudai
redcoder
```

```output2
No
```

```input3
abcdefghijklmnopqrstuvwxyz
ibyhqfrekavclxjstdwgpzmonu
```

```output3
Yes
```

## 戻幣
### 崙�s

- $ 1\ \leq\ |S|\ \leq\ 2\ \times\ 10^5 $
- $ |S|\ =\ |T| $
- $ S $, $ T $ は哂弌猟忖のみからなる

### Sample Explanation 1

肝のように荷恬を佩えば、`azzel` を `apple` にできます。 - $ c_1 $ として `e` を、$ c_2 $ として `l` を�xぶと、`azzel` が `azzle` になる - $ c_1 $ として `z` を、$ c_2 $ として `p` を�xぶと、`azzle` が `apple` になる

### Sample Explanation 2

どのように荷恬を佩っても `chokudai` を `redcoder` にできません。

