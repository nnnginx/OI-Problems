## ��Ŀ����
���ӳ������ˡ�

~(��<)~(��<)~(��<)~(��<)~(��<)~(��<)~(��<)~(��<)~(��<)~(��<)~(��<)~(��<)~(��<)~(��<)

![](https://cdn.luogu.com.cn/upload/image_hosting/0nqiwonz.png)

## ��Ŀ����
С �� ϲ����ʡ���ѧϰ��һ����ʷ�����

���ȣ���ӵ��һ����ģ�崮������Ϊ $s$��Ȼ������ѡ��һ�� $1 \le l \le r \le |s|$���� $s$ �ĵ� $l$ �� $r$ ���ַ�ɾ���������ߵ��ַ���ƴ����������õ���������ַ���Ϊ $s'$��

������������ѡ��һ���µ� $1 \le l' \le r' \le |s'|$��Ȼ���� $s'$ �ĵ� $l'$ �� $r'$ ���ַ���ɵ��ַ���Ϊ $s''$���������������ʾ��� $s''$��

���磬�����ģ�崮��Ϊ $s=\texttt{cciaohalloo}$����ôһ����ʷ����ǣ�ѡ�� $l=5$��$r=7$���õ� $s'=\texttt{ccialloo}$��Ȼ��ѡ�� $l'=2$��$r'=7$���õ� $s''=\texttt{ciallo}$��

����С �� ��һ����Ŀ�괮�� $t$������֪���ж����ֲ�ͬ�ķ���������ʹ�á�ģ�崮��$s$ ������� $t$���������ַ�����ͬ���ҽ���ѡ��� $l,r,l',r'$ ����ͬ��

## �����ʽ
�����У��ֱ�Ϊ�ַ��� $s$ �� $t$��

## �����ʽ
��һ�У����������Ŀ�괮��$t$ �ķ�������

```input1
aabbaaba
aba
```

```output1
23
```

```input2
ciaohallo
ciallo
```

```output2
2
```

```input3
babacbbaababbacbababbabbbaaabaabababbabbabababba
ababab
```

```output3
1535
```

```input4
sssssssssssssssssssssssssssssssssssss
sss
```

```output4
15470
```

```input5
abcbbbcbcbcbacbacbaaabcbcbcbaabacbca
cb
```

```output5
3995
```

## ��ʾ
### ���ݷ�Χ

**��������������**��

- Subtask 0��6 points����$|s| \le 400$��$|t| \le 200$��
- Subtask 1��10 points����$|s| \le 700$��$|t| \le 300$��
- Subtask 2��10 points����$\forall i,j,s_i=t_j$��
- Subtask 3��10 points����$|t|=1$��
- Subtask 4��20 points����$|s| \le 10^4$��$|t| \le 3 \times 10^3$��
- Subtask 5��14 points����$|t|=2$��
- Subtask 6��30 points�������������ơ�

�������в������ݣ�$1 \le |s| \le 4 \times 10^5$��$1 \le |t| \le 2 \times 10^5$��$s,t$ ֻ����СдӢ����ĸ��

