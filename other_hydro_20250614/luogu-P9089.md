## ��Ŀ����
���� $n$ ��**��Сд��ĸ���**���ַ���������� $i$ ���ַ����ļ�ֵΪ����������Ӵ���������**����ж��������ͬ���Ӵ�Ҳͳ�ƶ��**������ $i$ ���ַ�����һ���Ӵ������壬���ҽ�������Ӵ��ܱ��ֳ����ɸ���������ÿ���������� $n$ ���ַ���������һ���ַ���������һ����׺��

������һ�� $n=4$ �����ӣ�
```plain
int
printf
scanf
ntnt
```

- ���� `printf` ����ַ������ԣ�`intf` ��������ģ���Ϊ���Ա�ʾ�� `int` �� `f` ���ֱ��� `int` �� `scanf` �ĺ�׺���� `rint` ���ǡ�

- ���� `ntnt` ����ַ������ԣ�`ntnt` Ҳ��������ģ���Ϊ���Ա�ʾ�� `nt` �� `nt`�����Ƕ��� `int` ͬһ����׺�����߿��Ա�ʾ�� `ntnt`���� `ntnt` ��һ����׺��

���ڣ�С Z ��֪���� $n$ ���ַ�����ֵ֮�͡�

## �����ʽ
��һ��һ������ $n$��

֮�� $n$ �У�ÿ��һ���ַ�����

## �����ʽ
һ��һ����������ʾ��ֵ֮�͡�

```input1
4
int
printf
scanf
ntnt
```

```output1
23
```

```input2
4
ireallywanttobemissjiaransdog
butmissjiaransaidthatshelikedcatsandicried
iknowwhyicrywheniamneitheradognoracatbecauseimactuallyamouse
ineverexpectedmissjiarantolikeherselfiunderstandthatallpeopleliketounderstandthecutedogorcatthatyuyuusestomakemoneyandnoonelikesthemousewithwetandwetdiseases
```

```output2
391
```

## ��ʾ
#### ���ݹ�ģ��Լ��

**���⿪��������Ժ� O2 �Ż���**

�� $s_i$ ��ʾ�� $i$ ���ַ������ȡ�
| Subtask | ���ݷ�Χ/�������� | ��ֵ |
| :------: | :------: | :------: |
| $1$ |  $n\le 3$��$\sum\limits \lvert s_i\rvert\le10$| $5 \operatorname{pts}$ |
| $2$ | $n=26$��ÿ���ַ�������һ���ַ���� | $5 \operatorname{pts}$ |
| $3$ |$n=1$ | $15 \operatorname{pts}$ |
| $4$ | $\sum\limits \lvert s_i \rvert \le 2000$ | $15 \operatorname{pts}$ |
| $5$ | $\sum\limits \lvert s_i \rvert \le 2\times10^5$ | $30 \operatorname{pts}$ |
| $6$ | $\sum\limits \lvert s_i \rvert \le 10^6$ | $30 \operatorname{pts}$ |

���� $100\%$ �����ݣ�$1\le n \le 5\times10^5$��$n\le \sum\limits \lvert s_i \rvert \le 10^6$��

