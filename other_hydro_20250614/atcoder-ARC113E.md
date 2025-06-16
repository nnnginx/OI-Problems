## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/arc113/tasks/arc113_e

`a` �� `b` ����ʤ������� $ S $ ���뤨���ޤ���$ S $ �����¤β����� $ 0 $ �������R�귵���ƤǤ���Ǖ��**���**�������Ф����Ƥ���������

- ͬһ�����֤Ǥ��� $ S $ �� $ 2 $ �w�������֤��x�֡��������g�������Ф�ǰ�ᷴܞ�������x��� $ 2 $ ���֤��������롣���ʤ����$ S $ �� $ i $ ����Ŀ�� $ s_i $ �ȱ����Ȥˤ���С�$ s_i=s_j $ �ʤ� $ i\ <\ j $ ���x��� $ S $ �� $ s_1\dots\ s_{i-1}s_{j-1}\dots\ s_{i+1}s_{j+1}\dots\ s_{|S|} $ ���ä��Q���롣

�ʤ������Ά��}�Ǥϥƥ��ȥ��`���� $ T $ ���뤨���ޤ���$ i $ ��Ŀ�Υƥ��ȥ��`���������� $ S_i $ �Ǳ��졢$ S=S_i $ �ˌ�������ӛ�Ά��}��⤯���}�Ǥ���

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ T $ $ S_1 $ $ \vdots $ $ S_T $

## �����ʽ
$ T $ �г������衣$ i $ ��Ŀ�ˤϡ�$ S_i $ �˲����� $ 0 $ �������R�귵���ƤǤ���Ǖ�����������Ф�������衣

## ��Ŀ����
**��Ŀ����**

����ֻ��$a$,$b$��ɵ�һ���ַ���$S$������������²�������Σ�ʹ���յ��ַ����ֵ������

- ѡ��$S$��������ͬ���ַ���������֮����ַ�����ת����ɾ����ѡ��������ַ���

������$S$��ѡ������λ��$i,j(s_i=s_j,i<j)$������Խ��ַ���$S$�滻Ϊ$s_1\dots s_{i-1}s_{j-1}s_{j-2}\dots s_{i+2}s_{i+1}s_{j+1}s_{j+2}\dots s_{|S|}$

��$T$������

**�����ʽ**

��һ��һ������$T$.
������$T$�У�ÿ��һ���ַ���$S$.

**�����ʽ**

$T$�У�һ��һ���ַ�������ÿһ��������ݣ�����ֵ��������ַ�����

**���ݷ�Χ**

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

## ��ʾ
### �Ƽs

- $ 1\ \leq\ T\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ |S_i|\quad\ (i=1,\dots,\ T) $
- $ 1\ \leq\ |S_1|\ +\ \dots\ +\ |S_T|\ \leq\ 2\times\ 10^5 $
- $ S_i $ �� `a` �� `b` ����ʤ�

### Sample Explanation 1

\- $ 1 $ ��Ŀ�Υƥ��ȥ��`���ϡ�$ 1 $ ����Ŀ�� $ 4 $ ����Ŀ�ˌ����Ʋ������Ф����Ȥ� $ S $ �� `bba` �ˤǤ��ޤ��� - $ 2 $ ��Ŀ�Υƥ��ȥ��`���ϡ�$ 1 $ ����Ŀ�� $ 5 $ ����Ŀ�ˌ����Ʋ������Ф����Ȥ� $ S $ �� `bba` �ˤǤ��ޤ��� - $ 3 $ ��Ŀ�Υƥ��ȥ��`���ϡ�$ 1 $ ����Ŀ�� $ 2 $ ����Ŀ�ˌ����Ʋ������Ф����Ȥ� $ S $ �� `bbabaa` �ˤǤ��������� $ 3 $ ����Ŀ�� $ 5 $ ����Ŀ�ˌ����Ʋ������Ф����Ȥ� $ S $ �� `bbba` �ˤǤ��ޤ���

