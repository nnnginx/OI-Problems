## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc113/tasks/arc113_e

`a` と `b` からなる猟忖双 $ S $ が嚥えられます。$ S $ に參和の荷恬を $ 0 $ 指參貧�Rり卦してできる看����**恷寄**の猟忖双を箔めてください。

- 揖匯の猟忖である $ S $ の $ 2 $ �w侭の猟忖を�xぶ。それらの�gの猟忖双を念瘁郡��させ、�xんだ $ 2 $ 猟忖を��茅する。すなわち、$ S $ の $ i $ 猟忖朕を $ s_i $ と燕すことにすれば、$ s_i=s_j $ なる $ i\ <\ j $ を�xんで $ S $ を $ s_1\dots\ s_{i-1}s_{j-1}\dots\ s_{i+1}s_{j+1}\dots\ s_{|S|} $ で崔き�Qえる。

なお、この���}ではテストケ�`スが $ T $ ��嚥えられます。$ i $ ��朕のテストケ�`スは猟忖双 $ S_i $ で燕され、$ S=S_i $ に��して貧��の���}を盾く���}です。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ T $ $ S_1 $ $ \vdots $ $ S_T $

## 補竃鯉塀
$ T $ 佩竃薦せよ。$ i $ 佩朕には、$ S_i $ に荷恬を $ 0 $ 指參貧�Rり卦してできる看����恷寄の猟忖双を竃薦せよ。

## 籾朕寄吭
**籾朕宙峰**

公協峪喇$a$,$b$怏撹議匯倖忖憲堪$S$��低辛參恂參和荷恬販吭肝��聞恷嶮議忖憲堪忖灸會恷寄。

- 僉夲$S$議曾倖�猴�議忖憲��繍万断岻寂議忖憲堪鍬廬��旺評渠侭僉夲議曾倖忖憲。

曳泌壓$S$嶄僉夲曾倖了崔$i,j(s_i=s_j,i<j)$��低辛參繍忖憲堪$S$紋算葎$s_1\dots s_{i-1}s_{j-1}s_{j-2}\dots s_{i+2}s_{i+1}s_{j+1}s_{j+2}\dots s_{|S|}$

嗤$T$怏方象

**補秘鯉塀**

及匯佩匯倖屁方$T$.
俊和栖$T$佩��耽佩匯倖忖憲堪$S$.

**補竃鯉塀**

$T$佩��匯佩匯倖忖憲堪��斤耽匯怏霞編方象��補竃忖灸會恷寄議忖憲堪。

**方象袈律**

$
1\le T\le 2\times 10^5\\
1\le |S_i|(i=1,2\dots ,T)\\
1\le |S_1|+|S_2|+\dots +|S_T|\le 2\times 10^5
$

```input1
20
abbaa
babbb
aabbabaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbabaaaaabbaababaaabbabbbbbaaaaa
babbbaaaabaababbbabaabaaaaababaa
bbaababababbbaaabaabababaabbabab
abaabbabaabaaaaabaaaabbaabaaaaab
aabababbabbabbabbaaaabbabbbabaab
aabababbabbbbaaaabbaaaaabbaaaabb
abbbbaabaaabababaaaababababbaabb
aaaaaaaaaaaaaaaaaaaaaaabbbbbbbbb
aaaaaaaaaabbbbbbbbbbbbbbbbbbbbbb
abababaaababaaabbbbbaaaaaaabbbbb
aabbaaaaababaabbbbbbbbbaabaaabbb
babababbababbbababbbbbababbbabbb
bbbbababbababbbabababbabbabbbbbb
aaaaaaaaaaaaaaaaababababbbabbbbb
aabababbabbabababababababbbbabbb
```

```output1
bba
bba
bbba
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbaaaaaaaa
bbbbbbbbbbbbbaaaaaaa
bbbbbbbbbbbbbbbb
bbbbbbbbbb
bbbbbbbbbbbbbbbbab
bbbbbbbbbbbbbb
bbbbbbbbbbbbbabb
abbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbaaaaaaaaa
bbbbbbbbbbbbbbbaaaaa
bbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbba
bbbbbbbbbaaaaaaaaaaaaaaa
bbbbbbbbbbbbbbbbba
```

## 戻幣
### 崙�s

- $ 1\ \leq\ T\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ |S_i|\quad\ (i=1,\dots,\ T) $
- $ 1\ \leq\ |S_1|\ +\ \dots\ +\ |S_T|\ \leq\ 2\times\ 10^5 $
- $ S_i $ は `a` と `b` からなる

### Sample Explanation 1

\- $ 1 $ ��朕のテストケ�`スは、$ 1 $ 猟忖朕と $ 4 $ 猟忖朕に��して荷恬を佩うことで $ S $ を `bba` にできます。 - $ 2 $ ��朕のテストケ�`スは、$ 1 $ 猟忖朕と $ 5 $ 猟忖朕に��して荷恬を佩うことで $ S $ を `bba` にできます。 - $ 3 $ ��朕のテストケ�`スは、$ 1 $ 猟忖朕と $ 2 $ 猟忖朕に��して荷恬を佩うことで $ S $ を `bbabaa` にでき、その瘁 $ 3 $ 猟忖朕と $ 5 $ 猟忖朕に��して荷恬を佩うことで $ S $ を `bbba` にできます。

