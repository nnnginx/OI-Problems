## ��Ŀ����
```cpp
bool binary_search(int n, int p[], int target){
    int left = 1, right = n;
    while(left < right){
        int mid = (left + right) / 2;
        if(p[mid] == target)
            return true;
        else if(p[mid] < target)
            left = mid + 1;
        else
            right = mid - 1;
    }
    if(p[left] == target) return true;
    else return false;
}
```

������֪�������������ڴ���һ���������ݼ������� $\texttt p$ �� $\texttt{target}$ ������ $\texttt p$ �г��ֹ�����ô�᷵�� $\texttt{true}$��Ȼ������ $\texttt p$ �����ڵ�����ʱ��Ȼ��

���������� $n$ ��һ������ $b_1,\dots,b_n \in \{\texttt{true},\texttt{false}\}$�����ݱ�֤����һ�������� $k$��ʹ�� $n=2^k-1$��

�涨 $S(p)$ Ϊ $i \in \{1,\dots,n\}$ ʱ $\texttt{binary\_search(n, p, i)}$ ����ֵ��Ϊ $b_i$ �ĸ����������������һ�� $\{1,\dots,n\}$ ������ $p$��ʹ�� $S(p)$ ������С������������ֹ��򣩡�

## �����ʽ
**�����ж������ݡ�**

��һ��һ�������� $T$����ʾ����������

ÿ�����ݵĵ�һ�а���һ�������� $n$���ڶ��а���һ������Ϊ $n$ ���ַ�����ֻ�����ַ� `0` �� `1` ���޿ո񣩡����е��� $i$ ���ַ�Ϊ `1` ʱ���� $b_i=\texttt{true}$������ $b_i=\texttt{false}$��

## �����ʽ
��� $T$ �У�ÿ�������õ����� $p$��**Special Judge �������ʽҪ��ǳ��ϸ�ÿ����ĩ�����пո�ȶ����ַ���**

```input1
4
3
111
7
1111111
3
000
7
0000000
```

```output1
1 2 3
1 2 3 4 5 6 7
3 2 1
7 6 5 4 3 2 1
```

```input2
2
3
010
7
0010110
```

```output2
3 2 1
7 3 1 5 2 4 6
```

## ��ʾ
#### ���ֹ���

- ��һ���������е��������� $p$ ������ $S(p) \le 1$ ʱ���÷�Ϊ���������ֵܷ� $100\%$��
- ����һ���������е��������� $p$ ������ $0 \le S(p) \le \lceil \log_2 n \rceil$ ʱ���÷�Ϊ���������ֵܷ� $50\%$��

����������ֻ��ƣ�ÿ�����Ե��ʵ�ʵ÷�Ϊ��ʽ��ȡ���Ľ�������磬������������ܷ�Ϊ $3$ �Ҹ��������е��������� $p$ ������ $0 \le S(p) \le \lceil \log_2 n \rceil$ ʱ���÷�Ϊ $1$ ������ $1.5$��

#### ���� 1 ����

ǰ������������ $S(p)=0$��

������������ $S(p)=1$����Ϊ $\texttt{binary\_search(n, p, 2)}=\texttt{true} \neq b_2$��

������������ $S(p)=1$����Ϊ $\texttt{binary\_search(n, p, 4)}=\texttt{true} \neq b_4$��

#### ���� 2 ����

�������ݾ����� $S(p)=0$��

#### ���ݹ�ģ��Լ��

**�������������ԡ�**

- Subtask 1��3 pts����$b_i=\texttt{true}$��
- Subtask 2��4 pts����$b_i=\texttt{false}$��
- Subtask 3��16 pts����$1 \le n \le 7$��
- Subtask 4��25 pts����$1 \le n \le 15$��
- Subtask 5��22 pts����$n=2^{16}-1$ �� $b_i$ ���������
- Subtask 6��30 pts�������������ơ�

���� $100\%$ �����ݣ�$1 \le T \le 7000$��$1 \le \sum n \le 10^5$��$\forall n \in \{n|n=2^k-1,k \in \N^*\}$��

#### ˵��

�������� [eJOI2021](https://sepi.ro/ejoi/2021) Day 2 A BinSearch����ӭͨ��˽�Ż����ķ�ʽ�����б�д�� [Special Judge](https://www.luogu.com.cn/paste/5fdi0fvc) ���� hack��

