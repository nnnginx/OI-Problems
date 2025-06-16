## ��Ŀ����
**��Ŀ��Դ��**[link](https://www.gitlink.org.cn/thusaa/codeplus5)��



## ��Ŀ����
С V �տ������ˣ��������������е��Ագ���������������һ�� CP ����һ�¡�

��������ѡ��һ�����ݷ�Χ $N$������ $N$ ��һ��������

�������µĺ�����

```cpp
// rand_int(l, r) ���ر����� [l, r] �е�һ���������
vector<int> ans;

void solve(int l, int r) {
    if (l == r) {
        ans.push_back(r);
        return ;
    }
    int m = rand_int(l, r - 1);
    if (rand_int(0, 1) == 0) {
        solve(l, m);
        solve(m + 1, r);
    } else {
        solve(m + 1, r);
        solve(l, m);
    }
}
```

���ǳ�ʼ�� $\texttt{ans}$ Ϊ�գ���ô���� $\texttt{solve(1, N)}$ ֮��$\texttt{ans}$ ���洢һ�����С�

���ڵ������ǣ��������� $P$�����ж����ֲ�ͬ����������ɷ�������ʹ��� $\texttt{ans}$ �д洢������ǡ��Ϊ $P$��

����������������ɷ�ʽ�ǲ�ͬ�ģ����ҽ����ں���ĳ�ε��� $\texttt{rand\_int}$ ʱ������������������˲�ͬ������

�������� $998244353$ ȡģ��

## �����ʽ
��һ��һ�������� $N$����֤ $N\le 5\times 10^5$��

������һ�� $N$ ���������������� $\{P_i\}$��

## �����ʽ
���һ��һ����������ʾ�𰸡�

```input1
4
4 3 1 2
```

```output1
2
```

## ��ʾ
**���ݷ�Χ��**

$\def\arraystretch{1.21}
\begin{array}{|c|c|c|}\hline
\bold{\small{������}}&\textbf{score}&\textbf{constraints}\\\hline
\text{A}&20&N\le5000,P_i=N-i+1\\\hline
\text{B}&10&B\le10^5,P_i=N-i+1\\\hline
\text{C}&30&N\le10^5\\\hline
\text{D}&40&N\le5\times10^5\\\hline
\end{array}$

