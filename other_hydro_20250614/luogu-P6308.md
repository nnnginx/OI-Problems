## ��Ŀ����
������֪����¶ŵ�Ǳ�����

## ��Ŀ����
��¶ŵϣ��ά��һ������Ϊ $n$ ���������� $a$����ʼֵ��Ϊ $0$��

������¶ŵ��Ҫ���� $q$ �β�����ÿ��ѡ�������е�һ������ $[s,s+l-1]$ �������������� $w,k$��ʹ�����е� $i \in [1,l]$��$a_{s+i-1}$ ���� $w\times i^k$ ��  

��¶ŵ��ϣ�� $k$ �ܴ������������һ������ $m$������ $0\le k\le m$��

Ϊ�˲���ͷ�Լ򵥵���¶ŵ�е�������ֻ��Ҫ��� ���ν��������в����������е�ÿ�����ֶ� $2^{64}$ ȡģ���� $\text{unsigned long long}$ ��Ȼ�������Ľ�����ɡ�

Ϊ�˰�������õ�������⣬�������һ��α���룺

$$\def\b#1{\textbf{ #1 }}\def\t#1{\text{ #1 }}\def\s{\quad}
\def\l{\underline{\kern{300pt}}\cr[-10pt]}
\def\r{\overline{\underline{\kern{300pt}}}}
\begin{aligned}
&\r\cr&\b{Algorithm:}\t{An easy structure}\cr[-13pt]&\l\cr
&\begin{aligned}
    \t{1.}&\b{input}n,m,q \cr
    \t{2.}&\b{for}i=1\b{to} q \b{do} \cr
    \t{3.}&\s\b{input} s,l,w,k \cr
    \t{4.}&\s\b{for} j=1 \b{to} l \b{do}\cr
    \t{5.}&\s\s a[s+j-1] \gets a[s+j-1]+w\times \t{pow}(j,k) \cr
    \t{6.}&\s\b{end}\cr
    \t{7.}&\b{end}\cr
    \t{8.}&\b{for} i=1 \b{to} n \b{do}\cr
    \t{9.}&\s\b{output} a[i]\cr
    \t{10.}&\b{end}\cr
    \end{aligned}\cr[-12pt]
&\r\end{aligned}
%Made by @��ɢС���任�� .
%You can find his contributions by searching "JoesSR".
$$
���� $\rm pow(a,b)$ �ĺ���Ϊ $a^b$�� 

## �����ʽ
������·������ `input(n,m,q,S,L,W,K)` ������ $n,m,q,s_i,l_i,w_i,k_i$���±�**��һ��ʼ**��  

���� $s,l,w,k$ �ĺ�������Ŀ��������һ�¡�

## �����ʽ
������·������ `output(n,R)` ������������� $R_i$ Ϊ���в�������������У��±�**��һ��ʼ**��

```input1
10 0 5 233

```

```output1
6942214367

```

```input2
1000 9 500 6666

```

```output2
7636746723064426256
```

## ��ʾ
#### ����һ˵��

���ɵ�����Ϊ��
```plain
10 0 5
7 1 1558211206 0
1 3 401324017 0
4 5 235225636 0
6 4 2137131141 0
1 2 3791175968 0
```
���Ľ���ǣ�
```plain
4192499985 4192499985 401324017 235225636 235225636 2372356777 3930567983 2372356777 2137131141 0
```

---

#### ��������&�������

```cpp
typedef unsigned long long u64;
typedef unsigned int       u32;
u32 MT[624],idx;
void _init(u32 seed){
    MT[0]=seed; idx=0; for(int i=1;i<624;++i) 
    MT[i]=(0x6c078965*(MT[i-1]^((MT[i-1])>>30)+i));
}
void _gene(){
    for(int i=0;i<624;++i){
        int x=MT[i]&0x80000000+(MT[(i+1)%624]&0x7fffffff);
        MT[i]=MT[(i+397)%624]^(x>>1);
        if(x&2)MT[i]^=0x9908b0df;
    }
}
u32  _calc(){
    if(!idx) _gene(); int x=MT[idx];
    x^=x>>11,x^=(x<<7)&(0x9d2c5680);
    x^=(x<<15)&0xefc60000,x^=x>>18;
    idx=(idx+1)%624; return x;
}
u64 _get(){u64 ret=_calc()*_calc(); return ret;}
u64 _get(u64 _l,u64 _r){return _get()%(_r-_l+1ull)+_l;}
void input(int &_n,int &_m,int &_q,int *_S,int *_L,u64 *_W,int *_K){
    u32 seed; scanf("%d%d%d%u",&_n,&_m,&_q,&seed); _init(seed); int i=1;
    if(_n>100) for(;i<=_q/4;++i){
        int _a=_get(1,_n-100),_b=_get(_a+_m,_a+_m+1),_l=_b-_a+1,_k=_get(0,_m);
        u64 _w=_get(); _S[i]=_a,_L[i]=_l,_W[i]=_w,_K[i]=_k;
    }
    if(_n>100) for(;i<=_q/2;++i){
        int _a=_get(1,100),_b=_get(_n-100,_n),_l=_b-_a+1,_k=_get(0,_m);
        u64 _w=_get(); _S[i]=_a,_L[i]=_l,_W[i]=_w,_K[i]=_k;
    }
    for(;i<=_q;++i){
        int _a=_get(1,_n),_b=_get(1,_n); if(_a>_b) swap(_a,_b);
        int _l=_b-_a+1,_k=_get(0,_m); u64 _w=_get();
        _S[i]=_a,_L[i]=_l,_W[i]=_w,_K[i]=_k;
    }
}
void output(int n,u64 *R){
    u64 ret=n^_get(); for(int i=1;i<=n;i++) ret^=_get()+R[i];
    printf("%llu\n",ret);
}
```
���У����� `input()` �������ݣ����� `output()` ������ݡ�

**�������κ�ʱ����ó���`input`��`output`��ĺ�����������������ֻ�ܵ���һ��**��

--- 

#### ���ݷ�Χ 

�� $20$ �����Ե㣬��������������

$$\def\arraystretch{1.5}\begin{array}{|c|c|c|c|}\hline
\textbf{���} & n & m & q \\ \hline
[1,3] & \le 3\times 10^3 & =9 & \le 3\times 10^3 \\\hline
[4,5] & \le 3\times 10^5 & =0 & \le 3\times 10^5 \\\hline
[6,9] & \le 3\times 10^5 & =1 & \le 3\times 10^5 \\\hline
[10,13] & \le 3\times 10^5 & =2 & \le 3\times 10^5 \\\hline
[14,16] & \le 3\times 10^5 & =9 & \le 3\times 10^5 \\\hline
[17,20] & \le 5\times 10^5 & =9 & \le 1\times 10^6 \\\hline
\end{array}$$

���У�$[l,r]$ ��ʾ���Ϊ $l,l+1,\cdots,r-1,r$ �Ĳ��Ե㡣

���� $100\%$ �����ݣ����� $1\le l_i \le l_i+s_i-1 \le n,0\le k_i\le m,0 \le w\le 2^{64}-1$��

