## 【测评说明】
==测评未考察上机动手编程能力以及其他更多细节，因此每个课程除需要补未掌握课次外。还有如下更扎实的衔接建议-非强制：
如果要补期中前课次，建议+补期中训练；
如果要补期中后课次，建议+补期末训练；
如果涉及期中前后课次，且错3次课及以上，建议期中+总复习+期末；==

<br>1. 以下C++不可以作为变量的名称的是(   )。
{{ select(1) }}
- CCF GESP
- ccfGESP
- CCFgesp
- CCF_GESP
- 没有正确答案
- 我不知道

2. 设有 int a = 10 , b = 15，C++语句 cout <<  ( a - b ) && ( a < b ) 执行后的输出是(   )。

{{ select(2) }}
- 1
- 0
- true
- false
- 没有正确答案
- 我不知道




3.现有一个双精度浮点型变量 a ，请问下面哪个语句可以实现保留3位有效数字输出？（   ）
{{ select(3) }}
- scanf("%3d" , &a); 
- scanf("%3d" , a);
- printf("%.3lf", a);
- printf("%.3lf", &a);
- 没有正确答案
- 我不知道





4.下面C++代码执行时输入21后，有关描述正确的是（ ）。

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/719ps1m2h81k3s.png)

{{ select(4) }}
- 代码第4行被执行
- 第4和第7行代码都被执行
- 仅有代码第7行被执性
- 第8行代码将被执行
- 没有正确答案
- 我不知道





5.下面C++代码执行后的输出是（ ）

    int a = 0;
   	for(int i  = 0 ; i <= 10 ; i+=2)
          a = a + i;
  	cout << a;

{{ select(5) }}
- 28
- 30
- 32
- 34
- 没有正确答案
- 我不知道





6.选择正确的选项，实现输出n个正整数中的最大值。（   ）
```
 int n, a, max = -1; 
​	cin >> n; // n个正整数 
​	for(int i = 1; i <= n; i++)
​	{
  ​		cin >> a;
  ​		if( max < a)
​			________;
​	}
​	cout << max;
```

{{ select(6) }}
- max += a;
- max += i;
- max = a;
- max == a;
- 没有正确答案
- 我不知道



7.执行完下方代码后输出结果是（  ）
```
  int sum = 0 , i = 0;
​  while(i<10)
  {

  ​		i++;

      if(i % 2 == 0)
  			continue;
  ​		else if(i % 7 == 0)
  ​			break;
  		sum += i;
​   }
cout << sum；
```
{{ select(7) }}
- 1
- 4
- 9
- 16
- 没有正确答案
- 我不知道





8.在下列代码的横线处填写（ ），可以使得输出是正整数 1234 各位数字的平方和。

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/d9oo4um2h81k2r.png)

{{ select(8) }}
- n / 10
- (n / 10) * (n / 10)
- n % 10
- (n % 10) * (n % 10)
- 没有正确答案
- 我不知道






9.下列4个表达式中，答案不是整数8的是？（ ）

{{ select(9) }}
- abs(-8)
- min(max(8, 9), 10)
- int(8.88)
- sqrt(64)
- 没有正确答案
- 我不知道





10.C++表达式 int(-123.123 / 10) 的值是（ ）。

{{ select(10) }}
- -124
- -123
- -13
- -12
- 没有正确答案
- 我不知道







11.下列流程图的输出结果是（ ）

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/sbeo9sm2h81jcc.png)

{{ select(11) }}
- 5 12
- 12 5
- 5 5
- 12 12
- 没有正确答案
- 我不知道





12.下面C++代码执行后的输出是（ ）

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/zhtf3nm2h81ijn.png)

{{ select(12) }}
- 0
- 1
- 2
- 3
- 没有正确答案
- 我不知道





13.下面C++代码执行后的输出是（  ）。

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/nuruuym2h81ikh.png)

{{ select(13) }}
- 2#3#0
- 1#2#0
- 1#0#
- 2#3#
- 没有正确答案
- 我不知道





14.输入一行数，约定 1<= lineCount <= 9，输出以下图形。应在C++代码横线处填入（ ）。

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/vp6owum2h81ikm.png)

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/zhfeofm2h81ik9.png)

{{ select(14) }}
- (lineCount - i - 1) * 2
- (lineCount - i) * 2
- lineCount - i - 1
- lineCount - i
- 没有正确答案
- 我不知道





15.下列问题中不适合使用枚举算法解决的是（）

{{ select(15) }}
- 破解一个6位数密码
- 计算某个不大于1000的自然数的因子之和
- 查找100以内所有能被6整除且不能被10整除的数
- 查找一个不确定是大于100还是小于100的数
- 没有正确答案
- 我不知道





16.小明按照游戏规则，用程序随机生成一个整数（范围在1~6），表示一个骰子面向上的点数，并统计100次以内6朝上的次数，请问该过程运用了什么算法思想（）

{{ select(16) }}
- 枚举算法
- 模拟算法
- 骰子算法
- 递推算法
- 没有正确答案
- 我不知道





17.设有 int a[5] = {1 , 2 , 3 , 4 , 8};，问：元素3对应的下标为______。

{{ select(17) }}
- 1
- 2
- 3
- 4
- 没有正确答案
- 我不知道





18.小杨在做数学题，题目要求找出从1到35中能被7整除的数字，即[7, 14, 21, 28, 35]，则横线处应填入哪个代码？（ ）

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/ppljv8m2h81hsg.png)

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/gix7rem2h81h0w.png)

{{ select(18) }}
- arr[count++] = i;
- arr[i] = count++;
- arr[i] = count;
- arr[count] = count++;
- 没有正确答案
- 我不知道







19.以下为求 arr 数组前缀和数组的代码，空格处的代码应为（  ）。

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/gq8ob9m2h81h0o.png)

{{ select(19) }}
- presum[i] = arr[i-1] + arr[i];
- presum[i-1] = arr[i-1] + arr[i];
- presum[i] = presum[i-1] + arr[i]
- presum[i] = presum[i] + arr[i-1]
- 没有正确答案
- 我不知道





20.下列选项不正确的是（）

{{ select(20) }}
- char c1[10] = { 'a' , 'b' , 'c' , '\0' }; 和 char c2[10] = "abc"; 在输出时是一样的
- 定义char str[] = "abcd"，其中占用内存为5个字节
- 对于字符串“I am a student”，可用 cin 进行整个字符串的输入
- 使用scanf语句时，可使用格式控制符 %s 实现字符串的输入
- 没有正确答案
- 我不知道





21.设 char str1[10] = "abcdef"，str2[8] = "def" ，下面哪个选项可以比较 str1 和 str2 存储的字符串的大小？（    ）

{{ select(21) }}
- strcpy(str1, str2);
- strcat(str1, str2);
- strcmp(str1, str2);
- strlen(str1, str2);
- 没有正确答案
- 我不知道





22.执行下面的代码，输出结果是（    ）
```
string s1 = "abc", string s2 = "ac";
​if(s1 > s2)
  cout << s1+ s2;
else if(s1 < s2)
  cout << s2+s1;	
else
  cout << s1;
```

{{ select(22) }}
- abcac
- acabc
- abc
- ac
- 没有正确答案
- 我不知道





23.下列代码的输出结果是
```
int a = 4;
cout << a & 6;
```
{{ select(23) }}
- 4
- 6
- 10
- 1
- 没有正确答案
- 我不知道





24.一个二维数组定义为 int array[3][10]; ，假设int类型数据大小为4个字节，则这个二维数组最大占用内存为（ ）字节。

{{ select(24) }}
- 10
- 30
- 60
- 120
- 没有正确答案
- 我不知道





25.下面函数不能正常执行的是（）

{{ select(25) }}
- ![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/us1cynm2h81h0p.png)
- ![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/hznh0vm2h81h11.png)
- ![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/gks7akm2h81g95.png)
- ![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/2y4mrvm2h81fsn.png)
- 没有正确答案
- 我不知道





26.关于几种排序算法的说法，下面说法错误的是（ ）。

{{ select(26) }}
- 选择排序不是一个稳定的排序算法
- 冒泡排序算法不是一种稳定的排序算法
- 插入排序是一种稳定的排序算法
- 如果排序前2个相等的数在序列中的前后位置顺序和排序后它们2个的前后位置顺序相同，则称为⼀种稳定的排序算法
- 没有正确答案
- 我不知道





27.C++的内置函数 sort() 支持数组的局部排序。例如 int a={10,9,8,7,6,5,4,3,2,1} ，可以用
sort(a, a+5) ,排序结果是（） 

{{ select(27) }}
- {6,7,8,9,10,5,4,3,2,1}
- {1,2,3,4,5,6,7,8,9,10}
- {10,9,8,7,6,1,2,3,4,5} 
- {10,9,8,7,6,5,4,3,2,1} 
- 没有正确答案
- 我不知道



 

28.下面的C++程序中使用的算法是（ ）。

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/8z7eugm2h81fsl.png)

{{ select(28) }}
- 递推
- 递归
- 迭代
- 循环
- 没有正确答案
- 我不知道





29.在如下的C++代码执行后，设第11和12行的输出地址值分别为 X 和 Y ，则下面正确的是（ ）。

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/vzq9m7m2h81fs3.png)

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/dep6hcm2h81fra.png)

{{ select(29) }}
- X>Y
- X==Y
- X<Y
- 不确定
- 没有正确答案
- 我不知道





30.下列关于栈区的说法，错误的是？（）

{{ select(30) }}
- 栈区的内存由编译器自动分配与释放
- 程序中定义的所有变量都存储在栈区
- 当向栈区申请的内存空间超出栈区的内存时，程序会发生异常
- 栈区的大小在程序运行前就已经设定好了
- 没有正确答案
- 我不知道



31.假设变量 a 的地址是0x6ffe14，下⾯程序的输出是（ ）。

![img](https://wechatapppro-1252524126.cdn.xiaoeknow.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/m5awbkm2h81fsk.png)

{{ select(31) }}
- 10
- 0x6ffe14
- 0x6ffe15
- 0x6ffe18
- 没有正确答案
- 我不知道





32.下列关于C++语言中异常处理的叙述，正确的是（ ）。

{{ select(32) }}
- 一个 try 子句可以有多个 catch 子句与之对应。
- 如果 try 子句在执行时发生异常，就⼀定会进入某⼀个 catch 子句执行。
- 如果 try 子句中没有可能发生异常的语句，会产生编译错误。
- catch 子句处理异常后，会重新执行与之对应的 try 子句。
- 没有正确答案
- 我不知道
