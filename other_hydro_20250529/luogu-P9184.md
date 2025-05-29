## ��Ŀ����
Farmer John is interested in better interacting with his fellow cows, so he
decided he will learn the moo language!

## ��Ŀ����
Moo language is actually quite similar to English, but more minimalistic. There
are only four types of words: nouns, transitive verbs, intransitive verbs, and
conjunctions. Every two consecutive words must be separated by a space.  There
are also only two types of punctuation: periods and commas.  When a period or
comma appears after a word, it appears directly after the word, and is then
followed  by a space if another word appears next.

A sentence needs to follow one of the following formats:
- Type 1: noun + intransitive verb.
- Type 2: noun + transitive verb + noun(s). Specifically, at least one noun
must follow the transitive verb, and there must be a comma in front of every 
following noun besides the first following noun.

Two sentences may be joined into a compound sentence if a conjunction is placed
in between them.  The resulting compound sentence cannot be further joined with
other sentences or other compound sentences.  Every sentence (or compound
sentence, if two sentences are joined) must end with a period.

Farmer John has a word bank of $N$ words, $C$ commas, and $P$ periods. He may only use a word or punctuation mark as
many times as it appears in the word bank. Help him output a sequence of
sentences containing the maximum possible number of words.

Each input file contains $T$ independent instances of this
problem.


## �����ʽ
The first line contains $T$, the number of instances. Each instance is specified
as follows:

The first line consists of three integers $N, C$ and $P$.

The $N$ following lines will consist of two strings. The first string will be
the word itself that FJ can use (a string of at least $1$ and at most $10$ lowercase
letters), and the second string will be either one of the following: noun,
transitive-verb, intransitive-verb, or conjunction, denoting the type of the
word. It is possible the same word occurs more than once in FJ's word bank, but
it will always have the same type each time it appears.

## �����ʽ
In the first line, output the maximum possible number of words.

In the second line, output any sequence of sentences with the maximum possible
number of words. Any valid sequence will be accepted.

**The grader is sensitive to whitespace, so make sure not to output any
extraneous spaces, particularly at the end of each line.**

## ��Ŀ����
### ��Ŀ����

FJ ������ţ���õػ�������Ȥ������������ѧϰ moo ���ԣ�

### ��Ŀ����

moo ������Ӣ�����ƣ�����Ϊ�򵥡�����ֻ���������ͣ����ʡ����ﶯ�ʡ������ﶯ�ʺ����ʣ�ÿ��������֮������ÿո�����������Ž��������ź;�ţ�������ڵ��ʺ��棬���ñ����ź�����ڵ��ʣ�����Ҫ��һ���ո��ٷŵ��ʡ�

����ÿ�����ӣ�����Ҫ��ѭ���¸�ʽ�е�һ����

1. ����+�����ﶯ�ʡ�
2. ����+���ﶯ��+���ʣ������ж���������ﶯ�ʺ������������һ�����ʡ������ﶯ�ʺ���ĵ�һ�������⣬�����ÿ������ǰ�涼�����һ�����š�

Ҳ��������������֮���һ�����ʣ��γɸ��Ͼ䣬���Ͼ䲻���������������������ӡ�ÿһ�����ӣ��������Ͼ䣩�������Ծ�Ž�β��

FJ �Ĵʿ����� $N$ �����ʡ�$C$ �����ź� $P$ ����š�ÿ�����ʵ�ʹ�ô������ܳ�����������ڴʿ��г��ֵĴ��������ڣ���Ҫ�������������������Ҫ��ľ��ӣ�ʹ�ܵ����������ࡣ

ÿ�������ļ��й����� $T$ ��������

### �����ʽ

��һ������ $T$����ʾ��������������ÿ����������ʽ���£�

��һ���������������� $N$��$C$ �� $P$��

�ڽ������� $N$ �У�ÿ�����������ַ�������һ���ַ�������һ�� FJ �����õĵ��ʣ�ȫΪСд��ĸ������Ϊ $1$ �� $10$�����ڶ����ַ���Ϊ�����ַ����е�����һ������ʾ�õ��ʵ����ͣ�

- `noun`�����ʣ���
- `transitive-verb`�����ﶯ�ʣ���
- `intransitive-verb`�������ﶯ�ʣ���
- `conjunction`�����ʣ���

ͬһ�����ʿ����ڴʿ��г��ֶ�Σ�����ÿ�γ���ʱ���ǵ����Ͷ���ͬ��

### �����ʽ

��һ�������ɷ�������Ҫ��ľ������е���󵥴�����

�ڵڶ����У�����������У�ʹ��������ࡣ���⿪�� SPJ���κη�������Ҫ��ľ������о���ͨ����

**�벻Ҫ�������Ŀո���������ÿ��ĩβ��**

### ���ݷ�Χ

$1 \leq T \leq 100$��$1 \leq P, C \leq N \leq 10^3$��

- ���� 2-6��$N \leq 10$��
- ���� 7-11��$N \leq 100$��
- ���� 12-16��$N \leq 1000$��
- �����ų��� 5 �� 2 �Ĳ��Ե㣺û�м��ﶯ�ʡ�
- �����ų��� 5 �� 3 �Ĳ��Ե㣺û�в����ﶯ�ʡ�
- �����ų��� 5 �� 4 �Ĳ��Ե㣺û�����ʡ�

translated by [liyuanchen2021](https://www.luogu.com.cn/user/557680)

```input1
3
1 1 1
bessie noun
10 5 4
bessie noun
taught transitive-verb
flew intransitive-verb
elsie noun
farmer noun
john noun
and conjunction
and conjunction
nhoj noun
mooed intransitive-verb
24 5 4
but conjunction
bessie noun
taught transitive-verb
flew intransitive-verb
elsie noun
farmer noun
john noun
and conjunction
and conjunction
nhoj noun
mooed intransitive-verb
bob noun
impressed transitive-verb
cow noun
impressed transitive-verb
leaped intransitive-verb
elsie noun
bella noun
buttercup noun
pushed transitive-verb
mooed intransitive-verb
envy noun
john noun
nhoj noun

```

```output1
0

9
nhoj mooed. farmer taught elsie, bessie and john flew.
23
nhoj mooed. nhoj impressed john, farmer, elsie, bessie and cow impressed bob. bella pushed elsie and buttercup flew. envy mooed but john leaped.
```

## ��ʾ
$1\le T\le 100$��$1 \leq P,C\le N \leq 10^3$.

- Inputs 2-6: $N\le 10$.
- Inputs 7-11: $N\le 100$.
- Inputs 12-16: $N\le 1000$.
- Inputs with remainder 2 when divided by 5: There are no transitive
verbs.
- Inputs with remainder 3 when divided by 5: There are no intransitive
verbs.
- Inputs with remainder 4 when divided by 5: There are no conjunctions.

