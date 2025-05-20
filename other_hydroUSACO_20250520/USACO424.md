## Description  
�㡤л��С��ţ���ڻ���������־�����˴󽱣���������ũ��ᵽ�˳ǽ���һ�������С����������������������������ص�ԭ����ũ���䡣Ϊ�˻��������������Ϊ������������ţ���г�����������г���ר��Ϊţ����ƣ���  
���Լ��һ���ء�ͬ���ģ�������ͨ����ţ���г��ϣ�Ҫ�����ƽƽ���ȣ�Ҳ����һ�����׵��¡���ˣ�������ţ���г��ı��������������㲡�  
������ѡ��������ţ���г�ǰ�� F ��$1 \le F \le 5$�������ֺͺ��� R ��$1 \le R \le 10$�������֣�ʹ����  
$F\timesR$ ��ţ���г���������ı�׼��  
ǰ����ֵ��ͺţ��ݵ������������ڸ����ķ�Χ�ڡ�  
������ֵ��ͺţ��ݵ������������ڸ����ķ�Χ�ڡ�  
��ÿһ�ֳ�������У��������ʾ���ǰ����ֵĳ������Ժ�����ֵĳ������õ��̡�  
���Ĵ���������������С��������  
������ϵ�ת�����ʣ����ź�����������Ĳ�ĵķ������������ӣ� Ӧ�ôﵽ��С��  
��������Ĺ�ʽ����ƽ�����뷽�xi �������ݣ� ��  
### $$\bar{x}=\frac{1}{n}\sum_{i=1}^n x_i$$  
### $$F=\frac{1}{n}\sum_{i=1}^n (x_i-\bar{x})^2$$  
���㲢ȷ����ѳ�����ϣ����� F ��ǰ���֣�R ������֣���ʹ������С��  
  
> Having made a fortune on Playbov magazine, Hugh Heifer has moved from his original field in the country to a fashionable yard in the suburbs. To visit fond pastoral memories, he wishes to cowmmute back to his old stomping grounds. Being environmentally minded, Hugh wishes to transport himself using his own power on a Cowcycle (a bicycle specially fitted for his neatly manicured hooves).  
> Hugh weighs over a ton; as such, getting smoothly up to speed on traditional cowcycle gear sets is a bit challenging. Changing among some of the widely spaced gear ratios causes exertion that's hard on Hugh's heart.  
> Help Hugh outfit his Cowcycle by choosing F (1 <= F <= 5) gears (sprockets) in the front and R (1 <= R <= 10) gears in the rear of his F * R speed cowcycle subject to these rules:  
> The possible sizes (number of teeth) for the F front gears are specified.  
> The possible sizes (number of teeth) for the R rear gears are specified.  
> At any given gear setting, the gear ratio is the quotient of the number of teeth on the front gear and the number of teeth on the rear gear (i.e., number of front gear teeth divided by number of rear gear teeth)  
> The largest gear ratio must be at least three times the smallest.  
> The variance (see below) of the set of DIFFERENCES between successive (i.e., after sorting) gear ratios should be minimized.  
Calculate the mean and variance of a set of differences (xi in this formula) by the following formulae:  
> Deduce and print the optimal sets of F front gears and R rear gears so that the variance is minimized (and the ratios span a factor of at least 3x).  
  
## INPUT FORMAT  
��һ���� F �� R����ʾǰ���ֺͺ���ֵ�������  
�ڶ��а��� 4 �����֣�F1��F2��25 <= F1 < F2 <= 80����R1��R2��5 <= R1 < R2 <= 40������ F1 �� F2 �ͺŵ�ǰ���ֶ��ǿ��õģ��� R1 �� R2 �ͺŵĺ���ֶ��ǿ��õġ����ٻ���һ��Ϸ��Ľ⡣  
  
> The first line contains F and R, the numbers of front and rear gears. The second line contains four numbers: F1, F2 (25 <= F1 < F2 <= 80), R1, and R2 (5 <= R1 < R2 <= 40). All front gears from F1 through F2 are available; all rear gears from R1 through R2 are available. There will exist at least one legal set of gears.  
  
## SAMPLE INPUT  
```  
2 5  
39 62 12 28  
```  
## OUTPUT FORMAT  
�ڵ�һ�д�С�������ǰ���ֵ��ͺţ��ÿո�ֿ����ڵڶ��д�С�����������ֵ��ͺţ�ͬ���ÿո�ֿ�����Ȼ�����ֵĳ���һ����������  
����ж���⣬���ǰ���ֳ�����С����һ������һ�����ֳ�����С�ģ�����һ�����ֳ�����ȣ�����ڶ������ֳ�����С�ġ����������ƣ���������е�ǰ���ֳ�������ȣ���������İ취�������֣���ʵ���ǰѵ�һ�����ڶ����������ֱַ���Ϊ��һ���ڶ��������ؼ��������򣩡�  
  
> Display the number of teeth on the set of F chosen front gears, from smallest to largest, on the first line of output (separated by spaces). Display the number of teeth on the set of R chosen rear gears, from smallest  
to largest, on the second line of output. All gears have an integer number of teeth, of course.  
> If multiple optimal answers exist, output the answer with the smallest front gear set (smallest first gear, or smallest second gear if first gears match, etc.). Likewise, if all first gears match, output the answer  
with the smallest rear gear set (similar rules to the front gear set).  
  
## SAMPLE OUTPUT  
```  
39 53  
12 13 15 23 27  
```  
## Comment  
�������������ս���ǡ�������Ŀ��������������Ҫ��һ�����졣������������Ŀ�����ǵ�һ��һ��İ�������ȥ��  
����Ҫ�����ҳ�����ѳ�����ϡ���������������ӽ�ƽ��������ϡ���������Ĳ������ݣ�  
2 5  
39 62 12 28  
����ζ���� 2 ��ǰ���֣��ͺŷ�Χ�� 39..62 ��5������֣��ͺŷ�Χ�� 12..28���������������ǰ������ɵ�����ԣ��� 62-39+1=24 �ֳ��֣��������к������ɵ���Ԫ�飨�� 28-12+1=17 �ֳ��֣������������ѧԭ���ܹ��� 24!/22!/2! x 17!/5!/12! = 656,880 �ֿ��ܣ�������ô��Ϊ�ģ���  
����ÿһ�ֿ��ܣ�������ļ��㡣�ٸ�������˵������ö�ٵ��ĵ�һ�������ǰ������ 39 �� 40��������� 12��13��14��15 �� 16��  
���ȣ��������п��ܵĴ������ʣ�  
  
```  
39/12 = 3.25000000000000000000  
39/13 = 3.00000000000000000000  
39/14 = 2.78571428571428571428  
39/15 = 2.60000000000000000000  
39/16 = 2.43750000000000000000  
40/12 = 3.33333333333333333333  
40/13 = 3.07692307692307692307  
40/14 = 2.85714285714285714285  
40/15 = 2.66666666666666666666  
40/16 = 2.50000000000000000000  
```  
  
Ȼ�󣬶����ǽ�������  
  
```  
39/16 = 2.43750000000000000000  
40/16 = 2.50000000000000000000  
39/15 = 2.60000000000000000000  
40/15 = 2.66666666666666666666  
39/14 = 2.78571428571428571428  
40/14 = 2.85714285714285714285  
39/13 = 3.00000000000000000000  
40/13 = 3.07692307692307692307  
39/12 = 3.25000000000000000000  
40/12 = 3.33333333333333333333  
```  
  
Ȼ�󣬼����ľ���ֵ��  
  
```  
2.43750000000000000000 - 2.50000000000000000000 = 0.06250000000000000000  
2.50000000000000000000 - 2.60000000000000000000 = 0.10000000000000000000  
2.60000000000000000000 - 2.66666666666666666666 = 0.06666666666666666666  
2.66666666666666666666 - 2.78571428571428571428 = 0.11904761904761904762  
2.78571428571428571428 - 2.85714285714285714285 = 0.07142857142857142857  
2.85714285714285714285 - 3.00000000000000000000 = 0.14285714285714285715  
3.00000000000000000000 - 3.07692307692307692307 = 0.07692307692307692307  
3.07692307692307692307 - 3.25000000000000000000 = 0.17307692307692307693  
3.25000000000000000000 - 3.33333333333333333333 = 0.08333333333333333333   
```  
  
Ȼ�����ƽ�����ͷ��  
ƽ�����ǣ�������ô��Ϊ�ģ�0.0995370370370370370366666.�������Լ�� 0.00129798488416722��  
��Ȼ��������Ǵ���ģ���Ϊ������󴫶�����û�б���С�������ʴ�3����  
�ҳ�һ����ϣ�ӵ����С�ķ��ͬʱ��󴫶�������������С�������ʵ�3����  
  
> The challenge in this problem is "reading the problem". Don't read further if you are working on that level of challenge. If the problem is just completely unclear to you, read in.  
The problem wants you to find "an optimal set of gear ratios" such that the spacing between the ratios is most uniform. Consider the test case above:  
2 5  
39 62 12 28  
This specifies two front gears from the set 39..62; five rear gears from the set 12..28. The program must examine all possible pairs of 62-39+1=24 front gears and all possible quintuples from 28-12+1=17 rear  
gears. Combinatorically, The total number of possibilities is (24 take 2) times (17 take 5), which is 24!/22!/2! x 17!/5!/12! which is 656,880 possibilities (I think).  
For each of these possibilities, calculations like the following. This example considers in some sense the "first" case: front gears of 39 and 40, rear gears of 12, 13, 14, 15, and 16.  
First, calculate all the possible ratios:  
```  
39/12 = 3.25000000000000000000  
39/13 = 3.00000000000000000000  
39/14 = 2.78571428571428571428  
39/15 = 2.60000000000000000000  
39/16 = 2.43750000000000000000  
40/12 = 3.33333333333333333333  
40/13 = 3.07692307692307692307  
40/14 = 2.85714285714285714285  
40/15 = 2.66666666666666666666  
40/16 = 2.50000000000000000000  
```  
Then, sort them:  
```  
39/16 = 2.43750000000000000000  
40/16 = 2.50000000000000000000  
39/15 = 2.60000000000000000000  
40/15 = 2.66666666666666666666  
39/14 = 2.78571428571428571428  
40/14 = 2.85714285714285714285  
39/13 = 3.00000000000000000000  
40/13 = 3.07692307692307692307  
39/12 = 3.25000000000000000000  
40/12 = 3.33333333333333333333  
```  
Then, calculate the absolute value of the differences:  
```  
2.43750000000000000000 - 2.50000000000000000000 = 0.06250000000000000000  
2.50000000000000000000 - 2.60000000000000000000 = 0.10000000000000000000  
2.60000000000000000000 - 2.66666666666666666666 = 0.06666666666666666666  
2.66666666666666666666 - 2.78571428571428571428 = 0.11904761904761904762  
2.78571428571428571428 - 2.85714285714285714285 = 0.07142857142857142857  
2.85714285714285714285 - 3.00000000000000000000 = 0.14285714285714285715  
3.00000000000000000000 - 3.07692307692307692307 = 0.07692307692307692307  
3.07692307692307692307 - 3.25000000000000000000 = 0.17307692307692307693  
3.25000000000000000000 - 3.33333333333333333333 = 0.08333333333333333333  
```  
Then, calculate the mean and variance of the set of numbers on the right, above. The mean is (I think): 0.0995370370370370370366666. The variance is approximately 0.00129798488416722.  
Of course this set of gears is not valid, since it does not have a 3x span from highest gear to lowest.  
Find the set of gears that minimizes the variance and has a 3x or greater span.   