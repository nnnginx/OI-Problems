## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc082/tasks/abc082_b

哂弌猟忖のみからなる猟忖双 $ s $, $ t $ が嚥えられます。 あなたは、$ s $ の猟忖を挫きな��に�Kべ紋え、猟忖双 $ s' $ を恬ります。 また、$ t $ の猟忖を挫きな��に�Kべ紋え、猟忖双 $ t' $ を恬ります。 このとき、看����で $ s'\ <\ t' $ となるようにできるか登協してください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ s $ $ t $

## 補竃鯉塀
看����で $ s'\ <\ t' $ となるようにできるならば `Yes` を、できないならば `No` を竃薦せよ。

## 籾朕寄吭
公協$2$倖忖堪��$\color{blue}\text{海業<100}\color{red}\text{辛嬬嗤腎鯉}$����登僅頁倦辛參宥狛電會宸$2$倖堪聞誼$\color{purple}\text{及匯倖堪<及屈倖堪}\color{red}\text{(峺議頁忖灸會!)}$

```input1
yx
axy
```

```output1
Yes
```

```input2
ratcode
atlas
```

```output2
Yes
```

```input3
cd
abc
```

```output3
No
```

```input4
w
ww
```

```output4
Yes
```

```input5
zzz
zzz
```

```output5
No
```

## 戻幣
### 廣��

�Lさ $ N $ の猟忖双 $ a\ =\ a_1\ a_2\ ...\ a_N $ および�Lさ $ M $ の猟忖双 $ b\ =\ b_1\ b_2\ ...\ b_M $ について、看����で $ a\ <\ b $ であるとは、肝の $ 2 $ つの訳周のいずれかが撹り羨つことをいう;

- $ N\ <\ M $ かつ $ a_1\ =\ b_1 $, $ a_2\ =\ b_2 $, ..., $ a_N\ =\ b_N $ である。
- ある $ i $ ($ 1\ \leq\ i\ \leq\ N,\ M $) が贋壓して、$ a_1\ =\ b_1 $, $ a_2\ =\ b_2 $, ..., $ a_{i\ -\ 1}\ =\ b_{i\ -\ 1} $ かつ $ a_i\ <\ b_i $ である。 ただし、猟忖どうしはアルファベット��で曳�^される。

箭えば、`xy` $ < $ `xya` であり、`atcoder` $ < $ `atlas` である。

### 崙�s

- $ s $, $ t $ の�Lさは $ 1 $ 參貧 $ 100 $ 參和である。
- $ s $, $ t $ は哂弌猟忖のみからなる。

### Sample Explanation 1

箭えば、`yx` を `xy` と�Kべ紋え、`axy` を `yxa` と�Kべ紋えれば、`xy` $ < $ `yxa` となります。

### Sample Explanation 2

箭えば、`ratcode` を `acdeort` と�Kべ紋え、`atlas` を `tslaa` と�Kべ紋えれば、`acdeort` $ < $ `tslaa` となります。

### Sample Explanation 3

`cd`, `abc` をそれぞれどのように�Kべ紋えても、朕�砲鰡_撹できません。

