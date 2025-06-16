## ��Ŀ����
Little Johnny enjoys playing with words. He has chosen $n$ palindromes (a palindrome is a wordthat reads the same when the letters composing it are taken in the reverse order, such as dad, eye orracecar for instance) then generated all $n^2$ possible pairs of them and concatenated the pairs intosingle words. Lastly, he counted how many of the so generated words are palindromes themselves.

However, Johnny cannot be certain of not having comitted a mistake, so he has asked you to repeatthe very same actions and to give him the outcome. Write a programme which shall perform thistask for you.

TaskWrite a programme which:

reads the palindromes given by Johnny from the standard input,        determines the number of words formed out of pairs of palindromes from the input, which are palindromes    themselves,        writes the outcome to the standard output.


## �����ʽ
The first line of the standard input contains a single integer $n$, $n\ge 2$, denoting the number ofpalindromes given by Johnny. The following $n$ lines contain a description of the palindromes. The $(i+1)$'st line contains a single positive integer $a_i$ denoting the length of $i$'th palindrome and apalindrome of $a_i$ small letters of English alphabet. The number $a_i$ is separated from the palindromeby a single space. The palindromes in distinct lines are distinct. The total length of all palindromesdoes not exceed $2\ 000\ 000$.


## �����ʽ
The first and only line of the standard output should contain a single integer: the number of distinctordered pairs of palindromes which form a palindrome upon being concatenated.


## ��Ŀ����
### ��Ŀ����

Johnny ϲ����������Ϸ��

��д���� $n$ �����Ĵ��������Щ��������ϣ��ϲ���һ���´������׿�����һ������ $n^2$ ���´���

���������ʱ˳��������ģ��� `a` �� `b` ������ϳ� `ab` �� `ba`�������Լ����Լ����Ҳ������ġ�

��������֪����Щ�´����ж��ٸ����Ĵ������ܰ������

### �����ʽ

��һ��һ������ $n$��

������ $n$ �У��� $i$ �а���һ���� $a_i$ ��һ������Ϊ $a_i$ �Ļ��Ĵ���

��֤���д�ֻ����Сд��ĸ�������д�������ͬ�����л��Ĵ��ĳ��ȺͲ����� $2 \times 10^6$��

### �����ʽ

���һ�����������������������´���������

```input1
6
2 aa
3 aba
3 aaa
6 abaaba
5 aaaaa
4 abba
```

```output1
14
```

