## ��Ŀ����
Cornered at last, Bessie has gone to ground in a remote farm. The farm consists of $N$ barns ($2 \leq N \leq 10^5$) and $N-1$ bidirectional tunnels between barns, so that there is a unique path between every pair of barns. Every barn which has only one tunnel is an exit. When morning comes, Bessie will surface at some barn and attempt to reach an exit.

But the moment Bessie surfaces, the law will be able to pinpoint her location. Some farmers will then start at various exit barns, and attempt to catch Bessie. The farmers move at the same speed as Bessie (so in each time step, each farmer can move from one barn to an adjacent barn). The farmers know where Bessie is at all times, and Bessie knows where the farmers are at all times. The farmers catch Bessie if at any instant a farmer is in the same barn as Bessie, or crossing the same tunnel as Bessie. Conversely, Bessie escapes if she reaches an exit barn before any farms catch her.


Bessie is unsure about her chances of success, which depends on the number of farmers that the law is able to deploy. Given that Bessie surfaces at barn $K$, help Bessie determine the minimum number of farmers who would be needed to catch Bessie, assuming that the farmers distribute themselves optimally among the exit barns.


## �����ʽ
The first line of the input contains $N$ and $K$. Each of the following $N-1$ lines specify two integers, each in the range $1 \ldots N$, describing a tunnel between two barns.


## �����ʽ
Please output the minimum number of farmers needed to ensure catching Bessie.


## ��Ŀ����
### ��Ŀ����
���Bessie ����ȥ��һ��Զ����ũ�������ũ������ $N$ ���Ȳ֣�$2 \le N \le 10^5$���� $N-1$ �����������Ȳֵ�˫�����������ÿ�����Ȳ�֮�䶼��Ψһ��·����ÿ��ֻ��һ����������ĹȲֶ���ũ���ĳ��ڡ����糿���ٵ�ʱ��Bessie ����ĳ���Ȳ�¶�棬Ȼ����ͼ����һ�����ڡ�

���� Bessie ¶���ʱ������λ�þͻᱩ¶��һЩũ������ʱ���Ӳ�ͬ�ĳ��ڹȲֳ�������ץס Bessie��ũ��� Bessie ���ƶ��ٶ���ͬ����ÿ����λʱ���ڣ�ÿ��ũ�񶼿��Դ�һ���Ȳ��ƶ������ڵ�һ���Ȳ֣�ͬʱ Bessie Ҳ������ô������ũ���Ǻ� Bessie ����֪���Է���������������ʱ�̣�ĳ��ũ��� Bessie ����ͬһ���Ȳֻ��ڴ���ͬһ�������ũ��Ϳ���ץס Bessie������������� Bessie ��ũ����ץס��֮ǰ����һ�����ڹȲ֣�Bessie �Ϳ������ߡ�

Bessie ��ȷ�����ɹ��Ļ��ᣬ��ȡ���ڱ���Ӷ��ũ������������� Bessie ¶��ĹȲ�K������ Bessie ȷ��Ϊ��ץס������Ҫ��ũ�����С�������ٶ�ũ���ǻ��Լ�ѡ����ѵķ������������ǳ����ĳ��ڹȲ֡�

### �����ʽ

����ĵ�һ�а��� $N$ �� $K$���������� $N - 1$ �У�ÿ���������������� $1\sim N$ ��Χ�ڣ��������������Ȳֵ�һ�������

### �����ʽ

���Ϊ��ȷ��ץס Bessie �����ũ�����С������

�� @Marser �ṩ����

```input1
7 1
1 2
1 3
3 4
3 5
4 6
5 7
```

```output1
3
```

