<div>
<div id="problem-statement-preview">
<p>3  KHANS of Bollywood are planning to work together in a film called  "Three_Khans". Aamir (being perfect :P) wants the Alia to be a main  lead. But Alia (being very famous :P) is confused that whether to work in a  film or not. So they all have decided to play a game called  "Filmy_Sequence".</p>
<p>According to this game, Aamir will give any number to Alia to play  with it. Alia has to find two other numbers using it. That two numbers  represent Stardom of Salman and Srk. These two numbers shoud be found in such a  way so that both numbers will have same number of set ('1') bits in  their binary  representation as Aamir's number contains. One thing is also need to be  checked that Salman's number should be just next greater number to  Aamir's number and Srk's number should be just next smaller number to Aamir's  number (i.e in a order of their Stardom :P). They all have decided that  if  this "Filmy_Sequence" forms a G.P (Geometric Progression) then Alia has  to be in the favour of movie else not. Alia needs your help to find the  probabilty that she will work in a film and she also wants to find the  mean of the Stardum of Salman over Srk.</p>
<p>Note : All the three numbers should be positive and in a range upto 32 bits, and if not possible assume -1. (i.e if particular number is not possible with respect to Aamir's number, assume it as -1)</p>
<p><strong>Input Format :</strong></p>
<p>first line will have a number of numbers that Aamir will give (t) next t lines will have Aamir's number (n)</p>
<p><strong>Output Format :</strong></p>
<p>print the asked probability and mean. Any results within 10^-6 absolute error will be accepted.</p>
<p><strong>Constraints :</strong></p>
<p>t &lt;= 1000000</p>
<p>0 &lt;= n &lt;= 1000000</p>
<p><strong>Sample Input 1:</strong></p>
<p>3</p>
<p>1</p>
<p>2</p>
<p>3</p>
<p><strong>Sample Output 1:</strong></p>
<p>0.333333 4.000000</p>
<p><strong>Sample Input 2 :</strong></p>
<p>2</p>
<p>5</p>
<p>6</p>
<p><strong>Sample Output 2 :</strong></p>
<p>0.000000 3.500000</p>
<p><strong>Explanation :</strong></p>
<p>Case 2 : 5 -&gt; 3,5,6 and 6-&gt; 5,6,9 are the required numbers.</p>
</div>
</div>