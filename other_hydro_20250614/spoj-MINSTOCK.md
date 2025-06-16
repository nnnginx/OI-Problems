<p>Himanshu wants to invest into stock market and his friend Navneet helps him by providing him instruction for next <em>N</em>&nbsp;days.</p>
<p>&nbsp;</p>
<p>Navneet gives Himanshu 3 types of instruction,&nbsp;</p>
<p><strong>1 <em>X</em>&nbsp;<em>Y</em></strong>&nbsp; &nbsp; &nbsp; &nbsp;There is a stock X available at price Y. Here X is a string and Y is an integer.</p>
<p><strong>2 <em>X</em>&nbsp;<em>Z</em>&nbsp;</strong> &nbsp; &nbsp; &nbsp;The price of stock X has changed to Z. Here X is a string and Z is an integer.</p>
<p><strong>3 BUY</strong>&nbsp; &nbsp; &nbsp; Buy the stock which has the lowest price.</p>
<p>&nbsp;</p>
<p>You as a programmer, is given all the instructions of <strong><em>N</em>&nbsp;</strong>days. Can you tell,<strong> </strong><strong>which stock did Himanshu buy on which day</strong>. Print the output in same order as himanshu bought the stock. See sample Input and Output for Clarification.</p>
<p>&nbsp;</p>
<p><strong>At any point of time</strong>, there is <strong>atmost one stock of <em>X</em></strong>. However, <em>X</em>&nbsp;can be made available to market again through another instruction of type 1.</p>
<p><strong>All instructions are valid.</strong> i.e There is always some stock to buy having the minimum price of all. Also if the price of <em>X</em>&nbsp;has changed, then <em>X</em>&nbsp;is already known and hasn't been bought yet.</p>
<p>&nbsp;</p>
<h3><strong>INPUT&nbsp;</strong></h3>
<p>First line contains&nbsp;<em>N</em>. (1 ¡Ü&nbsp;<em>N</em>&nbsp;¡Ü 10<sup>6</sup>)</p>
<p>Next&nbsp;<em>N</em>&nbsp;lines, each of them contains an instruction of any of 3 types. (Look at instruction format above)</p>
<p>In any instruction, (X is a string of length upto 10 characters. All characters are from english alphabets, both small and capital )&nbsp;, and&nbsp; (0 ¡Ü&nbsp;<em>Y</em>&nbsp;¡Ü 10<sup>9)</sup>&nbsp;and (0 ¡Ü&nbsp;<em>Z</em>&nbsp;¡Ü 10<sup>9)</sup>&nbsp;.</p>
<p>&nbsp;</p>
<h3><strong>OUTPUT&nbsp;</strong></h3>
<p>For each instruction of type 3, output two values <em>X</em>&nbsp;and <em>Y</em>. Where <em>X</em>&nbsp;is the name of Stock having minimum price and <em>Y</em>&nbsp;is the day on which it was bought.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input :</strong>
<p>7</p><p>1 ABC 32</p><p>1 XDC 54</p><p>3 BUY</p><p>1 XCD 32</p><p>1 ABC 12</p><p>2 XDC 10</p><p>3 BUY</p><p>&nbsp;</p>
<strong>Output :</strong>
<p>ABC 3</p><p>XDC 7</p><p>&nbsp;</p></pre>
<h4><strong>Explanation</strong></h4>
<p>On day 3, there is instruction to buy. There are two stocks available "XDC" and "ABC", since price of "ABC" is less, he buys it. After this "ABC" is not available in market anymore.</p>
<p>On day 7, there is instruction to buy. Of all stocks available, "XDC" has the least price and hence he buys "XDC".</p>