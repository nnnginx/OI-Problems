<p><span style="font-family: 'Times New Roman'; font-size: medium;">The Association of Candy Makers is preparing to launch a new product. Its idea is old with a novel twist: it simply sells boxes of candies. But since people are what they consume and everyone wants to be unique these days, the ACM wants&nbsp;</span><em>every</em><span style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;candy box to be unique, in the sense that no two boxes should contain the same composition of candy types.</span></p>
<p style="font-family: 'Times New Roman'; font-size: medium;">The ACM is only able to make a small number n of different types of candy, but while limited in imagination, it is virtually limitless in resources, so it is able to produce as many as it wants of each type of candy. Furthermore, the candy types have different weights (though some may weigh the same), and in order to simplify pricing matters, the ACM wants all candy boxes to have the same total weight.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">With these restrictions, the ACM will only be able to make a limited number of boxes. For instance, if there are three types of candy, weighing 5, 5 and 10 grams respectively, 4 different boxes can be made with total weight 10 grams (using either two of type 1, or two of type 2, or one of type 3, or one each of types 1 and 2). The ACM would like to be able to make at least one box for everyone in the cosmos. So, given queries in the form of the number of people P in the cosmos, your job is to find the smallest possible total weight w such that P different boxes containing exactly w grams of candies can be made.</p>
<h1><strong>input</strong></h1>
<p style="font-family: 'Times New Roman'; font-size: medium;">The input consists of several data sets (at most 20). Each data set consists of four lines. The first line contains an integer 1 �� n �� 5, the number of candy types. The next line contains n integers w<sub>1</sub>, ..., w<sub>n</sub>, where 1 �� w<sub>i</sub>&nbsp;�� 10 is the weight (in grams) of the i:th candy type. The third line contains an integer 1 �� q �� 10, the number of queries. The last line of a data set contains q integers P<sub>1</sub>, ..., P<sub>q</sub>, where 1 �� P<sub>j</sub>&nbsp;�� 10<sup>15</sup>&nbsp;is the j:th query. Input is terminated by an incomplete data set where n = 0, which should not be processed.</p>
<h1><strong>output</strong></h1>
<p style="font-family: 'Times New Roman'; font-size: medium;">For the i:th data set, write a line&nbsp;<tt>"Set i"</tt>, followed by q lines giving, for each query P<sub>j</sub>, the minimal possible positive weight W<sub>j</sub>(in grams) of a candy box. If there is no weight W<sub>j</sub>&nbsp;such that at least P<sub>j</sub>&nbsp;candy boxes can be made, print&nbsp;<tt>"no candy for you"</tt>for that query. You may assume that W<sub>j</sub>, if it exists, will be at most 100 �� P<sub>j</sub>.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;"><strong>intput</strong></p>
<pre>3
5 5 10
1
4
4
3 1 4 2
2
142 700
1
10
1
100
0</pre>
<p><strong><span style="font-size: small;">output</span></strong></p>
<pre>Set 1
10
Set 2
23
42
Set 3
no candy for you</pre>
<pre></pre>
<p><strong>becarfull spoj watch you :  if i found anyone submit judge solution i will disqualify this submit .</strong></p>