<p><br> <img src="./23872/file/FT4yEL2F.png" alt="" width="undefined"></p>
<p>A very important aspect of web portals is customer reviews. The customers can rate any product  in the web portal. Generally, a customer can rate a product from one star to five star. Based on  the rating of all the customers the average customer rating for a product is shown. Look at the  figure on  the  left   to get  a clear   idea.  For example if three customers rate a  product   as   3   star,   4   star   and   4   star  respectively   then   the   average   rating  will be (3+4+4)/3 = 3.67 (Rounded to  two digits after the decimal point). In  the  figure on  the  left  847 customers  have rated a product and 597, 189, 26, 11 and 24 customers have rated the product as 5 star, 4  star,   3   star,   2   star   and   1   star   respectively.   So   the   average   rating   is:  <img src="./23872/file/zfbBwnB5.png" alt="" width="undefined"> (Rounded   to   eight   digits   after   the  decimal point).</p>
<p>Most web portals display the total number of people who have rated the product (As more people  rates  the product   the more reliable  the rating  is) but  do not  display  the numeric value of  the  average  rating.   In  the web portal  of  warzone  (A  renowned web portal)   the  total  number  of  customers that have rated a product (In the figure above the total 847 customers have rated the  product) and the average rating is stored in two different tables.  The average rating is stored,  rounded to n (0&lt;n&lt;9) digits after the decimal point so its value is not always the exact average  value. Unfortunately, the table that stored the total number of people that rated different products  somehow got  corrupted.  All   information available  in  the database now  is  the average  rating  (rounded  to at  most  eight  digits after   the decimal  point).  They do not  want   to  lose  the huge  number  of  customer   ratings  they have  received  throughout  10-15 years  but  also  they cannot  cheat with their customers by guessing the number of raters or voters. So from the average rating  they want   to determine  the minimum possible number  of people  that  rated  that  product.  You  have to help them find it out by writing a program.</p>
<h3>Input</h3>
<p>The input file can contain up to 2000 lines of inputs. Each line contains a non-negative floating- point number v (1 ¡Ü v ¡Ü 5). This number will have minimum one digit and maximum eight digits  after   the decimal  point.   If   this number  has n digits after   the decimal  point   then you have  to  assume that the value of the average is given rounded to n digits after the decimal point. Input is terminated by a line containing a negative number.</p>
<h3>Output</h3>
<p>For each line of input produce one line of output. This line contains the serial of output followed  by an integer T which denotes the minimum number of voter that is required for this average  rating.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>&nbsp;<pre>1.15
4.56316411
4.56316
3.67
3.66
-1.00</pre>
<strong>Output:</strong>&nbsp;
<pre>Case 1: 13
Case 2: 847
Case 3: 190
Case 4: 3
Case 5: 29</pre>
</pre>