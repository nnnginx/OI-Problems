## ��Ŀ����


Alice likes her digital alarm clock. She sets them up every evening. Last night Alice had a dream about her clock. Unfortunately, the only thing she is able to remember is the number of highlighted segments of the clock. Alice wonders what time was set on the clock in her dream.

Alice's clock have four digits: two for hours and two for minutes. For example, the clock below shows $9:30$ (note the leading zero).

![](https://cdn.luogu.com.cn/upload/image_hosting/6dl4fhwk.png)

The clock uses following digit representation.

![](https://cdn.luogu.com.cn/upload/image_hosting/igdzsez5.png)



## �����ʽ


The only line of the input file contains single integer $n$ �� the number of highlighted segments of the clock in Alice's dream $(0 \le n \le 30)$ .



## �����ʽ


Output five characters in $\text{hh:mm}$ format �� the time shown on the clock in Alice's dream. The time must be correct: $0 \le \text{hh} < 24$ and $0 \le \text{mm} < 60$ . If there are many possible correct times, output any of them. If there is none, output `Impossible`.



## ��Ŀ����
Alice�μ���һ��ʱ�䣬����ֻ�ǵ������ʱ���ڵ����������ֳ�����**����**�����ڸ���������������㷴��Alice�μ���ʱ�䣨���ж���𰸣��������һ�����ɣ�  
**����**����ش�Ҷ���˵���û��ƴ���ֵ���Ϸ������1Ҫ���������2Ҫ��5�����8Ҫ��7�����ȵȣ�����ĿͼƬ��ʾ���������**����**ָ�ľ���һ��ʱ���ÿһ�����֣���Ҫ��������ĺͣ�����09��30����Ҫ6+6+5+6=23����񣩡�  
**ʱ��**�����������ʱ�����Сʱ�ͷ��ӣ�����Сʱ��0��23֮�䣬������0��59֮��  

����һ������n��n��0��30���ڣ�����Alice�μ���**����**  
���һ���ַ���������кϷ���ʱ����������Ķ�������������ʱ�䣨�ж���������һ�����ɣ����������`Impossible`  

ע��ʱ���ǰ����



```input1
23

```

```output1
09:30

```

```input2
28

```

```output2
Impossible

```

```input3
2

```

```output3
Impossible

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 

spj provider: @[rzh123](user/237530)

