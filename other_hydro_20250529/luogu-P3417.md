## ��Ŀ����
The BBB (short for Byteotian Bit Bank) owns the largest net of cash dispensers in Byteotia. The clients of the BBB can draw their money from the cash dispensers on the basis of a cash card and a 4-digit PIN code. Lately, in order to increase their clients' security, the BBB has had a camera installed by each cash dispenser. The cameras transmit the recorded image to the BBB using radio signals. Unfortunately, the signals are being intercepted by a gang of computer thieves. The thieves attempt to discover the 4-digit PIN codes of the BBB clients, whose cash cards they subsequently steal. Being aware of this fact, the BBB clients try to perform redundant movements over the keyboard while entering the PIN. The camera is not able to pick out the keystrokes, it only records the finger movements. Consequently, it is usually not possible to determine the PIN unambiguously. For instance, the client moving his finger over the key 1 and then over the key 5 could have entered the following PIN codes: 1111, 1115, 1155, 1555, 5555. Desperate thieves glean the camera recordings, counting on being able to determine the PIN of a client or at least limiting the number of possible codes on the basis of multiple recordings of his transactions. Having accumulated sequences entered by a particular wealthy client of the BBB, they made you an "unnegotiable proposition".

TaskWrite a programme which:

reads from the standard input a description of the recorded sequences of finger movements, which the client has performed whilst entering his PIN,determines the number of distinct PIN codes, which the client can have (i.e. the number of those 4-digit PIN codes, which could have been entered by performing the given finger movement sequences),writes the outcome to the standard output.

BBB��Byteotian Bit Bank����д��ӵ��Byteotia�����Զ��������硣 BBB�Ŀͻ����Ը����ֽ𿨺�4λ����PIN����Զ���Ա������ȡ��������Ϊ����߿ͻ��İ�ȫ�ԣ�BBB�Ѿ���ÿ̨�Զ�������װ������������ʹ�����ߵ��źŽ���¼��ͼ���͵�BBB�����ҵ��ǣ���Щ�ź�����һȺ���Ե������ء�������ͼ����BBB�û���4λPIN�룬���������ȡ�����ǵ��ֽ𿨡���ʶ����һ��ʵ��BBB�û�����������PINʱִ�м����ϵ����ද�������ֻ�ܼ�¼��ָ�Ķ�������ˣ�ͨ����������ȷ��ȷ��PIN�롣���磬�û�����ָ�ƶ�����1�ϣ�Ȼ���ƶ�����5������������PIN�룺1111,1115,1155,1555,5555�������ĵ������ռ������¼�����ڵ����Ǹ���һ����ָ�ƶ����У�Ҫ����ȷ���û����Ծ��еĲ�ͬPIN���������

дһ������

�ӱ�׼�����ȡ��¼����ָ�ƶ����е��������û�������PIN��ʱִ�е���ָ�ƶ����У�ȷ���ͻ��˿��Ծ��еĲ�ͬPIN���������������Щ4λPIN��������������ͨ��ִ�и�������ָ�ƶ�˳����룩�������д���׼�����


## �����ʽ
The first line of the standard input contains a single integer $n$ denoting the number of recorded scenes depicting the action of entering the PIN by the client, $1\le n\le 1\ 000$. In the following $n$ lines there are descriptions of these scenes, a single one per line. The description of each scene consists of two positive integers separated by a single space. The first of those numbers, $t$, denotes the length of the sequence of movements, $1\le t\le 10\ 000$. The other is a $t$-digit number, whose consecutive digits denote consecutive keys, over which the client has moved his finger. The total length of all sequences does not exceed $1\ 000\ 000$.

��׼����ĵ�һ�а���һ������n����ʾ�û�����PIN�Ķ�������$1\le n\le 1\ 000$�� ������n���У�����Щ����������������ÿ������һ��������ÿ�������������������ɵ����ո�ֿ�����������ɡ� ��Щ���еĵ�һ������t��ʾ�˶����еĳ��ȣ�$1\le t\le 10\ 000$����һ����һ��tλ���������������������ֱ�ʾ�����ļ�����ʾ�û��ƶ�������ָ����Ŀ�ꡣ��֤$\sum t\le 1\ 000\ 000$��


## �����ʽ
The first and only line of the output should contain a single positive integer - the number of possible PIN codes of the client.

�����һ�У�Ӧ����һ�����������û����ܵ�PIN���������


```input1
2
3 123
3 234
```

```output1
5
```

