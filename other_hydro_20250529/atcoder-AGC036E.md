## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/agc036/tasks/agc036_e

`A`,`B`,`C` からなる猟忖双 $ S $ が嚥えられます。

$ S $ の�B�Aとは�泙蕕覆げ新崛� $ x $ であって、肝の訳周をすべて�困燭垢發里里Δ繊�恷�Lのものを $ 1 $ つ箔めてください。 なお、$ S $ の何蛍双とは、$ S $ から $ 0 $ ��參貧の猟忖を��茅して誼られる猟忖双を吭龍します。

- $ x $ に根まれる `A`,`B`,`C` それぞれの��方は畠て吉しい。
- $ x $ の嶄で揖じ猟忖は�Oり栽わない。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ S $

## 補竃鯉塀
訳周を�困燭貢鉗Lの何蛍双を $ 1 $ つ竃薦せよ。 盾が�}方ある��栽は、どれを竃薦しても屎盾とみなされる。

## 籾朕寄吭
公低匯倖海業葎 $n$ 議叙淫根ABC眉嶽忖銚議忖憲堪 $s$ ���嶬斷�低補竃匯倖諾怎和双勣箔議恷海議 $s$ 議徨會双:

+ ABC眉嶽忖憲議竃�峇諒��猴�。
+ 徨會双嶄�狒攸集�忖憲音嬬�猴�。

泌惚嗤謹怏盾��補竃販吭匯怏軸辛。

方象袈律��$|s|\leq 10^6$。

```input1
ABBCBCAB
```

```output1
ACBCAB
```

```input2
ABABABABACACACAC
```

```output2
BABCAC
```

```input3
ABCABACBCBABABACBCBCBCBCBCAB
```

```output3
ACABACABABACBCBCBCBCA
```

```input4
AAA
```

```output4

```

## 戻幣
### 崙�s

- $ 1\ \leq\ |S|\ \leq\ 10^6 $
- $ S $ は `A`,`B`,`C` からなる。

### Sample Explanation 1

$ S $ の何蛍双として、`ACBCAB` を深えると、これは訳周を�困燭靴討�り、またこれが恷�Lです。 また、`ABCBCA` も訳周を�困燭貢鉗Lの何蛍双です。 `ABCBCAB`, `ABBCCA` なども $ S $ の何蛍双ですが、これらは訳周を�困燭靴泙擦鵝�

### Sample Explanation 4

訳周を�困燭慌新崛个�腎猟忖双のみのこともあります。

