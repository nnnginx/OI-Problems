<!-- P { margin-bottom: 0.21cm; } -->
<p style="margin-bottom: 0cm">Courage (the cowardly dog) lives with his master Muriel and her husband Eustace in the city of Nowhere. Eustace is a farmer but not a very good one. One fine day Courage was taking a stroll in Eustace's cropless field when he found seeds of a magical tree. He seow them in the field and the next morning n magical apple trees grew on the previously cropless field. The number of apples on the ith tree is apples[i] (0&lt;=i&lt; n). The number of apples on a tree may change as sometimes courage eats some apples from a tree and sometimes apples grow instantly on the trees (because they are MAGICAL!!).</p>
<p style="margin-bottom: 0cm">Eustace wants to start a business of apples. So he frequently enquires Courage about the total number of  apples present on a range of trees. A range of trees is denoted by two integers, l and r (0&lt;=l&lt;=r&lt; n) and includes the trees from l to r (both inclusive).</p>
<p style="margin-bottom: 0cm">Courage is very loyal to Muriel and wants to keep some apples for her. So whenever Eustace asks about the total number of apples on a range, he deliberately doesn't count the apples on a tree, s, such that l&lt;=s&lt;=r and MIN(apples[l],apples[l+1],apples[l+2],...,apples[r])=apples[s].</p>
<p style="margin-bottom: 0cm">In other words, while calculating the sum of apples on the trees in a range, Courage doesn't include the apples on the tree that has the minimum number of apples in that range.</p>
<p>&nbsp;</p>
<p><strong>Input:&nbsp; </strong></p>
<p style="margin-bottom: 0cm">The first line contains n, the number of magical trees.</p>
<p>The second line contains n non-negative integers that denote the array apples.</p>
<p>The third line contains a non negative integer p, which is the number of events that take place.</p>
<p>&nbsp;Now follow p lines. Each line will be of the form 'EAT x y' or 'GROW x y' or 'COUNT x y'.</p>
<p>&nbsp;'EAT x y' means that Courage ate x apples from the yth tree. (0&lt;=y&lt; n)</p>
<p>&nbsp;'GROW x y' means that x apples grew magically on the yth tree (0&lt;=y&lt; n).</p>
<p>&nbsp;And 'COUNT l r' means that Eustace has told Courage to count the number of apples on the range of trees from l to r, both inclusive.</p>
<p>&nbsp;Remember that the trees are indexed from 0.</p>
<p><strong>Output:</strong></p>
<p>&nbsp;For each 'COUNT x y' event, output a single number that Courage tells to Eustace.</p>
<p style="margin-bottom: 0cm">&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1&lt;=n&lt;=100000</p>
<p>1&lt;=p&lt;=100000</p>
<p>0&lt;=apples[i]&lt;=10^9</p>
<p>0&lt;=l&lt;=r&lt;n</p>
<p>0&lt;=y&lt;n</p>
<p>The number of apples on a tree never exceeds 10^9.</p>
<!-- P { margin-bottom: 0.21cm; } -->
<p><strong>Sample Input: </strong></p>
<p style="margin-bottom: 0cm">10</p>
<p style="margin-bottom: 0cm">6 5  12  48 3 20 4 2 3 7</p>
<p style="margin-bottom: 0cm">6</p>
<p style="margin-bottom: 0cm">COUNT 2 4</p>
<p style="margin-bottom: 0cm">COUNT 7 9</p>
<p style="margin-bottom: 0cm">GROW 12 4</p>
<p style="margin-bottom: 0cm">COUNT 2 4</p>
<p style="margin-bottom: 0cm">EAT 6 9</p>
<p style="margin-bottom: 0cm">COUNT 7 9</p>
<p><strong>Sample Output:</strong></p>
<p style="margin-bottom: 0cm">60</p>
<p style="margin-bottom: 0cm">10</p>
<p>63</p>
<p>5</p>
<p style="margin-bottom: 0cm"><strong>SAMPLE TEST CASE EXPLANATION: </strong></p>
<p style="margin-bottom: 0cm">For 'COUNT 2 4', the sum of apples on trees 2,3 and 4 is 12+48+3=63. But as Courage doesn't include the apples on the tree with the minimum number of apples in the specified range (which in this case is the 4th tree), the number that he has to tell Eustace is 12+48=60.</p>
<p>For 'COUNT 7 9', the sum of apples on trees 7,8 and 9 is 2+3+7=12. In this case the tree with the minimum number of apples in the range is the 7th tree. So Courage tell Eustace the number 3+7=10</p>
<p>'GROW 12 4' means that the 4th tree, which has 3 apples, grows 12 more apples on it. So the number of apples on the 4th tree becomes 15.</p>
<p>For 'COUNT 2 4', the answer will be 48+15=63</p>
<p>'EAT 6 9' means that Courage eats 6 apples from the 9th tree. So the 9th tree now has 7-6=1 apple.</p>
<p>For 'COUNT 7 9,  the answer will be 2+3=5.</p>