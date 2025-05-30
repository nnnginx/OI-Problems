## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc118/tasks/arc118_d

殆方 $ P $ および屎の屁方 $ a,\ b $ が嚥えられます。 $ P $ ��からなる屁方双 $ A\ =\ (A_1,\ A_2,\ \ldots,\ A_P) $ であって、肝の訳周をすべて�困燭垢發里�贋壓するかを登協してください。 贋壓する��栽には、そのようなものをひとつ竃薦してください。

- $ 1\leq\ A_i\leq\ P\ -\ 1 $
- $ A_1\ =\ A_P\ =\ 1 $
- $ (A_1,\ A_2,\ \ldots,\ A_{P-1}) $ は、$ (1,\ 2,\ \ldots,\ P-1) $ を�Kべ紋えたものである
- 販吭の $ 2\leq\ i\leq\ P $ に��して、肝のうち富なくともひとつが撹り羨つ��
  - $ A_{i}\ \equiv\ aA_{i-1}\pmod{P} $
  - $ A_{i-1}\ \equiv\ aA_{i}\pmod{P} $
  - $ A_{i}\ \equiv\ bA_{i-1}\pmod{P} $
  - $ A_{i-1}\ \equiv\ bA_{i}\pmod{P} $

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられます。

> $ P $ $ a $ $ b $

## 補竃鯉塀
���}の訳周を�困燭衡�方双 $ A $ が贋壓するならば `Yes` を、そうでなければ `No` を竃薦してください。 `Yes` の��栽には、$ 2 $ 佩朕にそのような屁方双 $ A $ の光勣殆を、腎易で曝俳って 1 佩で竃薦してください。

> $ A_1 $ $ A_2 $ $ \ldots $ $ A_P $

訳周を�困燭衡�方双が�}方贋壓する��栽は、どれを竃薦しても屎盾となります。

## 籾朕寄吭
公協嵎方 $P$ 才曾倖屎屁方 $a,b$��勣箔更夛匯倖海業葎 $P$ 議會双諾怎��
- $1\le A_i\le P-1$��
- $A_1=A_P=1$��
- $(A_1,A_2,\dots,A_{P-1})$ 頁匯倖 $1\sim P-1$ 議電双��
- $\forall 2\le i\le P$��諾怎和双膨倖訳周嶄議崛富匯倖��
	1. $A_i\equiv aA_{i-1}\pmod P$��
    2. $A_{i-1}\equiv aA_i\pmod P$��
    3. $A_i\equiv bA_{i-1}\pmod P$��
    4. $A_{i-1}\equiv bA_i\pmod P$。

$\texttt{Data Range}:2\le P\le 10^5,1\le a,b\le P-1$��$P$ 葎嵎方。

Translated by pitham��蕩輿交鵝��。

```input1
13 4 5
```

```output1
Yes
1 5 11 3 12 9 7 4 6 8 2 10 1
```

```input2
13 1 2
```

```output2
Yes
1 2 4 8 3 6 12 11 9 5 10 7 1
```

```input3
13 9 3
```

```output3
No
```

```input4
13 1 1
```

```output4
No
```

## 戻幣
### 崙�s

- $ 2\leq\ P\leq\ 10^5 $
- $ P $ は殆方
- $ 1\leq\ a,\ b\ \leq\ P\ -\ 1 $

### Sample Explanation 1

$ P\ =\ 13 $ を隈として、 - $ A_2\equiv\ 5A_1 $ - $ A_2\equiv\ 4A_3 $ - $ \vdots $ - $ A_{13}\equiv\ 4A_{12} $ が撹り羨ち、この屁方双は訳周を�困燭垢海箸��_�Jできます。

