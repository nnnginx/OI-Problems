## ��Ŀ����


Famous programmer Gennady likes to create new words. One way to do it is to concatenate existing words. That means writing one word after another. For example, if he has words `cat` and `dog`, he would get a word `catdog`, that could mean something like the name of a creature with two heads: one cat head and one dog head.

Gennady is a bit bored of this way of creating new words, so he has invented another method. He takes a non-empty prefix of the first word, a non-empty suffix of the second word, and concatenates them. For example, if he has words `tree` and `heap`, he can get such words as `treap`, `tap`, or `theap`. Who knows what they could mean?

Gennady chooses two words and wants to know how many different words he can create using his new method. Of course, being a famous programmer, he has already calculated the answer. Can you do the same?



## �����ʽ


Two lines of the input file contain words chosen by Gennady. They have lengths between $1$ and $100 000$ characters and consist of lowercase English letters only.



## �����ʽ


Output one integer -- the number of different words Gennady can create out of words given in the input file.



## ��Ŀ����
### ��Ŀ����

�����ĳ���Ա Gennady ϲ�������µ��ʡ�����һ�ַ������������е��ʡ�

�ٸ����ӣ���� Gennady �� `cat` �� `dog` �����ʣ���ô����õ�һ���´ʣ� `catdog`���������ζ�Ŵ�������ͷ����������֣�һ��èͷ��һ����ͷ��

Gennady �������ִ����µ��ʵķ�ʽ�е����ģ��������������һ�ַ�����ʹ�õ�һ�����ʵķǿ�ǰ׺���ڶ������ʵķǿպ�׺�����������������������磬������е��� `tree` �� `heap` ������Եõ����� `treap`��`tap` �� `theap` ֮��ĵ��ʡ�

Gennady ѡ�����������ʣ�����֪��������ʹ���·����������ٸ���ͬ�ĵ��ʡ���Ȼ����Ϊ�����ĳ���Ա�����Ѿ�������˴𰸡���ͻȻ�뿼���㣬��ô���ܱ�дһ������Ѵ𰸼��������

### �����ʽ

���У�ÿ����һ�� Gennady ѡ��ĵ��� $s_i$ ��$1\leq |s_i| \leq 100000$��$s_i$ ����СдӢ����ĸ��ɣ���

### �����ʽ

���һ�����������������ʾ Gennady ���Դ������������ĵ����д�����ͬ���ʵ�������

```input1
cat
dog

```

```output1
9

```

```input2
tree
heap

```

```output2
14

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 



