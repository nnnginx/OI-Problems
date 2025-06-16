<div>
<div id="problem-statement-preview">
<p>Alia wants to play with you. She will give you a string (MSG) where ((N = length of MSG) &lt;= 10000)and multiple queries(M). Each query consists of an integer value K.</p>
<p>For each query you have to find the Kth substring if all the  substrings of the given string are arranged in lexicographically  increasing order without any duplicates( no substring will appear twice  in the given arrangement). You have to output the starting index of the Kth substring and it's  size. If the found substring has duplicates then(substring occurs  multiple times in the given string), output the smallest index where it  occurs.</p>
<p>If the no. of substring in the arrangement is less than the value of K, output -1.</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= size of string(MSG) &lt;= 10000</p>
<p>1 &lt;= No of queries (M) &lt;= 100000</p>
<p>1 &lt;= K &lt;= total number of substrings (not necessarily unique) of MSG;</p>
<p>Note : you have to output indexes as 1-based.</p>
<p><strong>input:</strong></p>
<p>The first line of input will consist of your string and no of queries(M), seperated by a space. Next M lines will consist of integer K (as mentioned in the problem).</p>
<p><strong>output:</strong></p>
<p>Your output should consist of M lines as per the answer for each query.</p>
<p><strong>Sample input:</strong></p>
<p>aaaaa 3</p>
<p>1</p>
<p>2</p>
<p>3</p>
<p><strong>Sample output :</strong></p>
<p>1 1</p>
<p>1 2</p>
<p>1 3</p>
<p><strong>Explanation:</strong></p>
<p>Our arrangement here will consist of substrings in the following order (a),(aa),(aaa),(aaaa),(aaaaa)</p>
<p>So 1st substring will be "a" and it's occuring at multiple index - (1,2,3,4,5) out of which the smallest  index is 1 and it's size is 1. Hence the answer will be (1,1).</p>
<p>The same will be for the other two queries.</p>
</div>
</div>