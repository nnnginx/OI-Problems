## ��Ŀ����
Garuda Team, I've got some good news. 

The chemical agent used as a catalyst for their WMD is being transported to our shores from the Estovakian mainland. 

This catalyst has already been carried into the outskirts of Gracemeria. 

As a measure of caution against any attempts to destroy it, it has been concealed at Fort Norton in Gracemeria's north. 

If we start advancing again, the enemy will most likely bring the catalyst into Gracemeria at a faster pace. 

If in fact weapons of mass destruction are used on the population of Gracemeria, the resulting devastation can't be expressed in enough words. 

It will lead to unspeakable tragedies. 

We've used this intelligence to come up with a solid proposal on how to prevent this scorched earth policy from being executed in our capital.

Just a minute ago, we received a letter of approval for our prevention plan from the Joint Chiefs of Staff. 

The proposal we put on the table for our scorched earth prevention policy is really quite simple. 

While the enemy transport unit is stationed at Fort Norton, **we'll ambush them.** 

We like to call it our tactic for pre-emptive victory. 

The enemy has loaded this catalyst into their transport vehicles and is able to send them into Gracemeria at any time. 

This plan will be carried out by a handful of our top pilots under absolute secrecy. 

**Fly through Fort Norton's canyon at an extremely low altitude to avoid radar detection, and take out those transport vehicles.** 

We've determined that a high-risk mission of this magnitude could not be executed by anyone other than Garuda Team. 

We're counting on a flawless execution here.

$$_{{\frac{\large\text{ACE COMBAT }\Large6}{\tiny{\text{F i r e s\quad O f\quad L i b e r a t i o n}}}}}\\ \text{Mission 12} \\\Large\text{Weapons of Mass Destruction}\\\tiny -\textit{ Boiling Point }-$$

![](https://cdn.luogu.com.cn/upload/image_hosting/3e1iqxjw.png)

## ��Ŀ����
Ϊ�˴ݻٵз�װ���� WMD �߻����ĳ��ӣ�����Ҫ�ڳ��Ϳմ��� Fort Norton ��Ͽ���Խӽ����ǡ�

Fort Norton ����Ϊ**ƽ������������ $y$��$y\in[0,10^7]$�������Էֶκ���** $A(y):y\mapsto x$ �Լ� $B(y):y\mapsto x$�����ж�������ʵ�� $y\in [0,10^7]$��**���� $A(y) \le B(y)$**��

������ F-15E ����Ϊһ�ʵ㣬**��ʼλ���� $(X_1,0)$**����֤ $A(0)\leq X_1\leq B(0)$��**ͬʱ���г��ٶ� $(v_0,\theta_0)$����ʾ���ٵĴ�С�ͷ���**��

Ϊ�˱���з����֣��㲻�ܴ��ʿ�������������Ķ����պ��㹻�ڱ���ƽ�ɵ�ʱ�򱣳����١�

��Ȼ�����ת���������� Ace Combat �����ǣ����ת��ȫ���� PSM ��ɡ�������˵����ķ��й켣ӦΪһ���������߶���ɵ����ߡ�������ת���л��ܵ�������**�������ı��Ľ���ı�ǰ�ĽǵĲ�ľ���ֵΪ $\alpha$�����ٶȴ�С���С $\alpha$**������㲻�ı䷽����ô���һֱ������ֱ���˶���

���� Ghost Eye ���ż������������**��� $y$ ���������ʱ�����**��

ͬʱ������Ҫ��֤������ʱ�̣������ڵ�λ�� $(x,y)$ ���� $A(y)\le x\le B(y)$��

PSM ת��Ĺ��غܴ��������Ҫ��֤**ת����������� $\bf 3\times 10^6$**��~~������ͻ��� Prez һ�� g-LOC ��һͷ�����Ǳ����ϡ�~~

���κ�һ��ת�򷽰���ʹ�����˶��� $(X_2,10^7)$ �ϣ�**�����ٶȲ������˶������б�Ϊ $\bf0$ ����**����ͬʱת����������� $3\times 10^6$�����Ƶģ���֤ $A(10^7)\leq X_2\leq B(10^7)$��

## �����ʽ
��һ���ĸ����� $n,m,X_1,X_2$ ������ʵ�� $v_0,\theta_0$��

**��֤ $v_0\pm 10^{-6}$ ��Χ�ڽ�����Բ��䡣**

������ $n$ �У�ÿ���������� $x,y$����֤ $y$ ��������һ�� $y$ �� $0$�����һ�� $y$ �� $10^7$������Щ���������߶������������õ����� $A$��

������ $m$ �У�ÿ���������� $p,q$ ��ʾ���� $B$���� $A$ �����뷽ʽͬ��

## �����ʽ
�����һ�� `1`��

Ȼ�������������˶��켣һ����һ�����ߣ���������Ҫ����һ������˵��� $K$����������� $K$ �У�ÿ������ʵ����ʾ����˵�����ꡣ����������ĵ����� $C:\{(s_1,t_1),(s_2,t_2),\cdots,(s_K,t_K)\}$����ô��ʾ $\forall i\in [1,K)$��$C_iC_{i+1}$ ֮�����ߣ��õ������߾�����������˶��켣��

����Ҫ��֤��

- $C_1$ �� $X_1$ �غϣ�$C_K$ �� $X_2$ �غϣ�
- **$C$ �� $y$ ���굥����**
- �������� $1\leq i<K$���� $t_i<t_{i+1}$��
- �������������ϵĵ� $(x,y)$������ $A(y)-10^{-6}\leq x\leq B(y)+10^{-6}$��
- �˶��������ٶȴ��� $0$��
- $K\leq 3\times10^6$��

�������ȷ�����һ�ַ�������Ҫ��ķ�����������Ϊ Accepted��������Ϊ Wrong Answer������в�ֹһ�ַ������������һ�ֽԿɡ�

**���⿪�� Special Judge��**

```input1
5 4 4000000 9000000 13 0
3000000 0
1000000 1000000
2000000 4000000
6000000 8000000
7000000 10000000
5000000 0
4000000 2000000
6000000 6000000
10000000 10000000
```

```output1
1
4
4000000.0000000000 0.0000000000
3000000.0000000000 2000000.0000000000
4000000.0000000000 6000000.0000000000
9000000.0000000000 10000000.0000000000
```

## ��ʾ
�������ͣ���С $10^6$ ������

![](https://cdn.luogu.com.cn/upload/image_hosting/5g98x901.png)

**ע���ʵ����˶������п��������߽磬Ҳ�������ű߽��˶�һ�Ρ�**

---

���� $100\%$ �����ݣ���֤ $2\leq n,m\leq 10^6$��$0\leq x,y,p,q\leq 10^7$��$x_1\leq X_1\leq p_1$��$x_n\leq X_2\leq p_m$��$0\leq \theta_0<\pi$��$0\leq v_0\leq 10^9$��

���� $100\%$ �����ݣ�ʵ�����Ȳ����� $12$ λ��

���� $100\%$ �����ݣ�**�� ֤ �� ��**��


- Subtask 1��3 pts����$n,m\leq 6$��$v_0\ge 50$��
- Subtask 2��8 pts����$n,m\leq 6$��
- Subtask 3��17 pts����$n,m\leq 200$��
- Subtask 4��13 pts����$n,m\leq 1500$��
- Subtask 5��17 pts����$n,m\leq 5000$��
- Subtask 6��19 pts����$n,m\leq 10^5$��
- Subtask 7��23 pts�������������ơ�

**��ע�⸡�������Ч�ʡ�**

---

idea��Sol1��solution��Sol1 & w33z8kqrqk8zzzx33��code��Sol1��data��w33z8kqrqk8zzzx33

