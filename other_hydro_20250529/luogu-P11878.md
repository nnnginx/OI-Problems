## ��Ŀ����
2024 �� 9 �� 11-22 �գ��� 45 ������������ƥ�����������������׶�������˹���С�С������Ϊһ���������尮���ߣ��������й�ע���ⳡ������

![](https://cdn.luogu.com.cn/upload/image_hosting/pe4k7psf.png)

 _ͼע���ڵ����ֱ����У��й�ѡ��Τ��սʤ������ѡ�֣������й����� 2.5:1.5 �ıȷ�սʤ��������_ 

���ڣ�С��Ҫ�������һЩ�����Ĺ�������֪ʶ��

1. �����������̹��� 8 �� 8 �У�**��������**�� $a \sim h$ ��ʾ�У�**���¶���**�� $1 \sim 8$ ��ʾ�У�
2. ÿ������һ��������һ���ʺ��������������������Լ��˸�������ʼ�������£�
   ![](https://cdn.luogu.com.cn/upload/image_hosting/jx82759s.png)
3. �������Թ�������ͬһ�С�ͬһ�С�ͬһб����**һ����**��λ�ã����磺
   ![](https://cdn.luogu.com.cn/upload/image_hosting/vr3q36zs.png)
   
   *ͼע�������Ĺ�����Χ����ͷ��ʾ���ܹ�������λ��*
4. �ʺ���Թ�������ͬһ�С�ͬһ�С�ͬһб����**�������**��λ�ã����磺
   ![](https://cdn.luogu.com.cn/upload/image_hosting/0rotqghv.png)
   ![](https://cdn.luogu.com.cn/upload/image_hosting/2iwr4258.png)
5. ����Թ���������"L"�͵�λ�ã���û��"�����"���ƣ����磺
   ![](https://cdn.luogu.com.cn/upload/image_hosting/j13m76k7.png)
6. ����Թ�����ͬһб����������ڵ�λ�ã����磺
   ![](https://cdn.luogu.com.cn/upload/image_hosting/8rldzs2a.png)
7. �����Թ�����ͬһ�С�ͬһ����������ڵ�λ�ã����磺
   ![](https://cdn.luogu.com.cn/upload/image_hosting/vga2ifsj.png)
8. �����Թ�����ǰ��������б��һ���ڵ�λ�ã����磺
   ![](https://cdn.luogu.com.cn/upload/image_hosting/xo2fdlh3.png)
9. �������ڶԷ�ĳ�����ӵĹ�����Χ��ʱ��������������check�������磺
   ![](https://cdn.luogu.com.cn/upload/image_hosting/m3qj07yf.png)
   
   *ͼע����ʱ�ڷ��������ڰ׷��ʺ�Ĺ�����Χ�ڣ��ڷ�������*

����ʹ�� FEN ��ʽ����һ�����档FEN ��ʽ��һ���ַ��������а��� 7 ��б�ܣ�/�������ַ�����Ϊ 8 ������ $s_{1..8}$�����У�$s_1$ ��Ӧ�� $8$ �е����ݣ�$s_2$ ��Ӧ�� $7$ �е����ݣ��Դ����ơ����� $v = s_i$��$v_1$ ��ʾ�� $a$ �е����ݣ�$v_2$ ��ʾ�� $b$ �е����ݣ��Դ����ơ�

��ע�⣬$v$ �ĳ��Ȳ�һ������ 8��

������ `R` ��ʾ�׷��ĳ���`N` ��ʾ�׷�����`B` ��ʾ�׷�����`Q` ��ʾ�׷��Ļʺ�`K` ��ʾ�׷�������`P` ��ʾ�׷��ı����ַ���Сд��ʽ��Ӧ�ڷ������ӡ�

���ַ����л������ $1 \leq i \leq 8$ �����֣���ʾ���������� $i$ ��û�����ӵĿո�

���磬������һ�����棺
   ![](https://cdn.luogu.com.cn/upload/image_hosting/psnnis20.png)

���Ӧ�� FEN Ϊ `r1bq1rk1/pppp1ppp/2n2n2/2b1p3/2B1P3/1P3N2/PBPP1PPP/RN1Q1RK1`��

���ڣ�С��������һ��ʹ�� FEN �����ľ��棬������������Ƿ���һ�����ڱ�������״̬��


## �����ʽ
��һ������һ�������� $t$����ʾ���������

������ $t$ �У�ÿ������һ������ FEN ��ʽ���ַ��� $s$����ʾһ���Ϸ��ľ��档

�����������ݣ����㣺$1 \leq t \leq 10$���Ҿ����в�����˫��ͬʱ�������������

## �����ʽ
�� $t$ �С�

�� $i$ ������� $i$ ����������������׷������������ `check`������ڷ������������ `CHECK`�����������һ������������� `none`��

```input1
9
1nb1n1r1/1r1kp2p/1PpP2p1/6b1/P4NPP/N2R4/R1PPQP2/q1B1KB2
4k1nr/r2pbqpp/2n2B2/pb1p4/p4P2/8/2PPPNPP/R2QKB1R
2b3nr/rp1pb1Qp/4pk2/2p5/P2qPP1P/3B4/RPnP2R1/1NB2KN1
rn3k1r/1pRb1p1p/3b2p1/pB1pp2q/3PP3/P1P1nP2/1PK1Q3/RNB3N1
r1b1kb2/1pppn1p1/p4p1r/4P3/8/1n1P2R1/P1PKP3/RNBQ1B2
r1b3r1/p3bp1p/1p2p1pn/2p1kP2/1PPn3P/P2PpKP1/R3P1B1/1Nq3NR
3qkb1r/p1p1pn1Q/1rn1b3/3PP1p1/1p4p1/NP3P2/P2P2BP/R1B1K1NR
rnb1k1r1/p1qpbp2/2p2pp1/1p2P2Q/1P3PP1/P2P1N1K/2P5/1RB2B1R
r4bnk/ppp1pb2/5QPr/3pP3/q1Pn4/P2p4/1P1P1P1P/1RB1K1NR

```

```output1
none
none
CHECK
check
check
check
none
none
CHECK

```

```input2
3
r1bqkb2/pp1nnp1r/3Np2p/2p5/1P1P3p/P4P2/2PBP1P1/R2QKBNR
2r4r/2N1nk1n/pp2b2p/2pq1pP1/1PPpP1P1/7P/P2PK3/R1B2BNR
2b1k2r/3r2pp/3b4/1P6/p1B1p3/P3nN1q/1n1P1PR1/1RB2K2

```

```output2
CHECK
none
check

```

```input3
3
3k4/8/5P2/p3N3/P3N2p/3K4/8/7r
3k4/8/5P2/p3N3/P3N2p/3K4/8/3r4
r1bqkb1r/pppp1Qpp/2n2n2/4p3/2B1P3/8/PPPP1PPP/RNB1K1NR

```

```output3
none
check
CHECK

```

## ��ʾ
���ڵ�������������������ֱ�������ʾ��
![](https://cdn.luogu.com.cn/upload/image_hosting/c8gdly9e.png)
![](https://cdn.luogu.com.cn/upload/image_hosting/y656nxud.png)
![](https://cdn.luogu.com.cn/upload/image_hosting/uq352kqv.png)

