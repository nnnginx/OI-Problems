## ��Ŀ����
Happybob ����һ��������������һ�� $n$ �� $n$ �е�б�����εĹ�����һ����������Լ���Ĵ�С���ܳ���б�����εĴ�С��

����ԭ�����ޣ���� Happybob �ļ�������� $m$ �������θ��Ƕ��ɵġ�

Happybob ��֪�������������������ļ��������Ƕ��١�

---

**��ʽ�����⣺**

�� $m$ �������θ��Ǵ�СΪ $n$ ��б�����Σ���า�Ƕ��ٸ����ӣ�

**б�����κ͸��ǵĶ����˵��/��ʾ**��


## �����ʽ
��һ�У�һ������ $T$����ʾѯ������

������ $T$ �У�ÿ���������� $n,m$����ʾһ��ѯ�ʡ�


## �����ʽ
$T$ �У�ÿһ�б�ʾһ��ѯ�ʵĴ𰸡�


```input1
3
5 1
6 2
8 2
```

```output1
9
20
32
```

## ��ʾ
### ����˵��

����ѯ�ʵķ����ǣ�

![3](https://cdn.luogu.com.cn/upload/image_hosting/m8uup5uc.png)

![4](https://cdn.luogu.com.cn/upload/image_hosting/70a01fpj.png)

![5](https://cdn.luogu.com.cn/upload/image_hosting/lypuap4t.png)

��������Ψһ��

### ���ݷ�Χ

$1\le T\le 50$��$1\le n\le 2\times 10^9$��$1\le m\le\lceil\dfrac{n}{2}\rceil$��

---

### ��ʽ������

**б�����εĶ��壺**

����ʽ���أ�����ֱ������ϵ������һ����СΪ $n$ ��**б������**��**����**Ϊԭ�㡣

�� $n$ Ϊ���������**б������**��������Ϊ������ $\big\{(x, y) \big | |x| + |y| \le \lfloor \frac{n}{2} \rfloor \text{ and } x, y \in \Z\big\}$ �еĵ�Ϊ**������**���ĵı߳�Ϊ $1$ ��**�����θ���**��ɵ����ͼ�Ρ�

�� $n$ Ϊż�������**б������**��������Ϊ������ $\big\{(x, y) \big | |x| + |y| \le \frac{n}{2} \text{ and } (x + \frac{1}{2}), (y + \frac{1}{2}) \in \Z\big\}$ �еĵ�Ϊ**������**���ĵı߳�Ϊ $1$ ��**�����θ���**��ɵ����ͼ�Ρ�

һ�� $n=5$ ��б�����Σ�����ɫΪ�������ģ���

![1](https://cdn.luogu.com.cn/upload/image_hosting/b633qef0.png)

һ�� $n=6$ ��б�����Σ�����ɫΪ�������ģ���

![2](https://cdn.luogu.com.cn/upload/image_hosting/bzq2por3.png)

**���Ƿ����Ķ��壺**

����һ�������� $R$ ���Ǹ�**б������**�����ҽ��� $R$ Ϊ������**����**��ɵĳ����Ρ�

������һ������б�����εĳ����Σ�

![3](https://cdn.luogu.com.cn/upload/image_hosting/7d0jsymo.png)

������**����**����б�����εĳ����Σ�

![4](https://cdn.luogu.com.cn/upload/image_hosting/2e2374s3.png)

![5](https://cdn.luogu.com.cn/upload/image_hosting/5j8wnvgb.png)

![6](https://cdn.luogu.com.cn/upload/image_hosting/rrxxe2ps.png)

����һ��**����**�����ǣ����ҽ���ѡ��� $m$ ������**б������**�ĳ�������������һ����ȫ�����ø��ӡ�


