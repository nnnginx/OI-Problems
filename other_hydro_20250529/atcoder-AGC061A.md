## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/agc061/tasks/agc061_a

塘双 $ A_1,\ \ldots,\ A_N $ があり、はじめ畠ての $ i $ について $ A_i\ =\ i $ です。返�� $ \mathrm{shuffle}(L,\ R) $ を參和として協�xします。

- $ R\ =\ L\ +\ 1 $ なら、$ A_L $ と $ A_R $ の�､鯣襪賁罎┐峠K阻する。
- そうでないなら、$ \mathrm{shuffle}(L,\ R\ -\ 1) $ を�g佩してから $ \mathrm{shuffle}(L\ +\ 1,\ R) $ を�g佩する。

$ \mathrm{shuffle}(1,\ N) $ を佩うとします。返���K阻瘁の $ A_K $ の�､魍�薦してください。

光秘薦ファイルについて、テストケ�`スを $ T $ ��盾いてください。

## 補秘鯉塀
秘薦は、���僻訌Δ�ら參和の侘塀で嚥えられる。

> $ T $ $ case_1 $ $ case_2 $ $ \vdots $ $ case_T $

光ケ�`スは、參和の侘塀である。

> $ N $ $ K $

## 補竃鯉塀
$ T $ 佩竃薦せよ。$ i $ 佩朕に、$ i $ ��朕のテストケ�`スの基えを竃薦すること。

## 籾朕寄吭
## 籾朕宙峰

低嗤匯倖電双海業葎 $n(n\le10^{18})$ 議電双 $A$��兜兵 $A_i=i$���嶬擽塰�序佩匯肝 $\mathrm{shuffle}(1,n)$ 荷恬。$\mathrm{shuffle}(L,R)$ 議協吶泌和��
- $ R\ =\ L\ +\ 1 $ 扮��$\mathrm{swap}(A_L,A_R)$
- 倦夸��卆肝峇佩 $\mathrm{shuffle}(L,R-1)$, $\mathrm{shuffle}(L+1,R)$

艇俶勣箔竃 $ \mathrm{shuffle}(1,\ n) $ 峇佩頼穎朔��$A_k (1\le k\le n)$ 議峙。慌 $T$ 怏方象。

```input1
7
2 1
2 2
5 1
5 2
5 3
5 4
5 5
```

```output1
2
1
2
4
1
5
3
```

## 戻幣
### 崙�s

- $ 1\ \leq\ T\ \leq\ 1000 $
- $ 2\ \leq\ N\ \leq\ 10^{18} $
- $ 1\ \leq\ K\ \leq\ N $

### Sample Explanation 1

$ N=2 $ のときは、參和を佩って $ A=(2,1) $ を誼ます。 - $ \mathrm{shuffle}(1,\ 2) $ を�g佩し、$ A_1 $ と $ A_2 $ を秘れ紋える。 $ N=5 $ のときは、參和を佩って $ A=(2,4,1,5,3) $ を誼ます。 - $ \mathrm{shuffle}(1,\ 5) $ を�g佩する。 - $ \mathrm{shuffle}(1,\ 4) $ を�g佩する。 - $ \mathrm{shuffle}(1,\ 3) $ を�g佩する。 - $ \vdots $ - $ \mathrm{shuffle}(2,\ 4) $ を�g佩する。 - $ \vdots $ - $ \mathrm{shuffle}(2,\ 5) $ を�g佩する。 - $ \mathrm{shuffle}(2,\ 4) $ を�g佩する。 - $ \vdots $ - $ \mathrm{shuffle}(3,\ 5) $ を�g佩する。 - $ \vdots $

