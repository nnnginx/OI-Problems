## 题目描述  
有时候程序员有很奇怪的方法来隐藏他们的口令。Binny会选择一个字符串S（由N个小写字母组成，5<=N<=5,000,000），然后他把S顺时针绕成一个圈，每次取一个做开头字母并顺时针依次取字母而组成一个字符串。这样将得到一些字符串，他把它们排序后取出第一个字符串。把这个字符串的第一个字母在原字符串中的位置-1做为口令。  
如字符串alabala，按操作的到7个字符串，排序后得：  
  
```  
aalabal  
abalaal  
alaalab  
alabala  
balaala  
laalaba  
labalaa  
```  
  
第一个字符串为aalabal，这个a在原字符串位置为7，7-1=6，则6为口令。  
## 输入格式：  
第一行：一个数：N  
第二行开始：字符串：S（每72个字符一个换行符）  
## 输出格式：  
一行，为得到的口令  
## 输入样例#1：   
```  
7  
anabana  
```  
## 输出样例#1：   
```  
6  
```  
## 说明  
题目满足：  
30%的数据n<=10000  
70%的数据n<=100000  
100%的数据n<=5000000  