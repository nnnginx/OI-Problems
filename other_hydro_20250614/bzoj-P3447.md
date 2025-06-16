


## 题目描述
  想象一下火车有N个座位，N个座位相当于数轴上的１至Ｎ共Ｎ个整点，第1个座位在整点1处，第2个座位在整点2处，。。。第N个座位在整点N处。 有N个奶牛排好队，要登陆坐火车，第N头奶牛在数轴的整点0处，第N-1头奶牛在数轴的整点-1处，。。。。第1头奶牛在数轴的整点-N+1处。第i头奶牛的座位号是Si。注意：每头奶牛都有唯一的一个座位，不会出现多头奶牛有相同的座位号。 
<span style="font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman"">在每一秒钟，奶牛会向右移动一步到达下一个整点，前提是没有奶牛挡住它。 <span style="font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman"">当第i<span style="font-family:
宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:"Times New Roman"">头奶牛到达它的座位Si<span style="font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman"">时，它需要花费Ti<span style="font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman"">秒去把行李放到头顶的行李架上，然后坐到自己的位置上，在次过程中，由于火车通道很窄，所以在第i<span style="font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman"">头奶牛坐到自己座位之前，在它左边的所有奶牛都不能动，要等奶牛i<span style="font-family:宋体;mso-ascii-font-family:"Times New Roman";
mso-hansi-font-family:"Times New Roman"">放好行李坐好后才能动。      
<span style="font-family:宋体;mso-ascii-font-family:"Times New Roman";mso-hansi-font-family:
"Times New Roman"">现在的问题是，至少要多少秒之后，所有的奶牛都能做到自己的座位上？ 
## 输入格式
 第一行，一个整数N。1 <= N <= 200000。 
 接下来有N行，第i行有两个整数Si和Ti,表示第i头奶牛的参数。所有Ti之和不超过10^9。    
## 输出格式
一个整数。 

```input1
3
2 5
3 10
1 5

```

```output1
19
 
```

## 提示
 OUTPUT DETAILS: After one step, they will all move 1 to the right and cow 3 will reach her seat: 123 123 Cow 3 takes 5 seconds to sit down, at which point she effectively disappears. 12 123 It takes 3 more seconds for cows 1 and 2 to reach their desired seats: 12 123 It takes 5 seconds for cow 1 to sit down and 10 seconds for cow 2 to sit down, so that's 10 seconds total. In total this took 1 + 5 + 3 + 10 = 19 seconds. 
## 题目来源
Gold


