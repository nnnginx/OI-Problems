<p>Blue Mary is a typist of some secret department.Now she has to type in many passwords in an hour,each of which has a fixed length: 6.Of course,the less times she presses the keyboard,the happier she is.</p>
<p>Unfortunately,the keyboard to type in the password is extraordinary designed to keep secrets.The keyboard has 6 particular keys instead of 10 number keys.To explain the usages of these keys,let's define the 6 position on the screen 1,2,3,4,5,6 from left to right.The keys' usages are shown below:</p>
<div>
<ul>
<li> Swap0: swap the digit in the cursor position and the digit in position 1.The cursor doesn't move.If the cursor is now in position 1,the digits on the screen won't be changed. </li>
<li> Swap1: swap the digit in the cursor position and the digit in position 6.The cursor doesn't move.If the cursor is now in position 6,the digits on the screen won't be changed. </li>
<li> Up: increase the digit in the cursor position by 1.If the digit in the cursor position is 9,no change will happen. </li>
<li> Down: decrease the digit in the cursor position by 1.If the digit in the cursor position is 0,no change will happen. </li>
<li> Left: move the cursor one position left.If the cursor is in position 1,no change will happen. </li>
<li> Right: move the cursor one position right.If the cursor is in position 6,no change will happen.</li>
</ul>
</div>
<p>At start,6 random digits will be given on the screen,and the cursor will in position 1.After some smart presses,she can type in the correct password,at that time the cursor position is unimportant.</p>
<p>Here is an example("()"denotes to the cursor):</p>
<pre>key pressed       screen
                  (1)23456
Swap1             (6)23451
Right             6(2)3451
Swap0             2(6)3451
Down              2(5)3451
Right             25(3)451
Up                25(4)451
Right             254(4)51
Down              254(3)51
Right             2543(5)1
Up                2543(6)1
Swap0             6543(2)1
</pre>
<p>Now Mary wants to know the minimal number of keys she has to press.Can you help her?</p>
<h3>Input</h3>
<p>The first line contains a single integer t(about 1000).t lines follow,each contains two 6-digit string,which show the digits on the screen at start and the password Mary is to type in,separated by a single space.</p>
<h3>Output</h3>
<p>t lines,each contains a single integer - the answer.</p>
<h3>Example</h3>
<pre><strong><tt>Sample input:</tt></strong>
1
123456 654321

<strong><tt>Sample output:</tt></strong>
11
</pre>
<p><strong>Added some new test data.</strong></p>