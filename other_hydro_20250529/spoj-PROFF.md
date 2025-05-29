<p>Professor farouk asked his students to create a variable of type integer and let it equal to 2147483647&nbsp;then asked them to add 1 for this variable they found that the answer like that -2147483648 while it should be 2147483648. One of students said that we can use long and other said we can use Big Integer&nbsp;in java, but for sure professor farouk know all this things but he wanted to ask what will you do if there's no data type&nbsp;can have your result ?<br> one of sudents gave the best answer he said we can add multi-digit numbers from right-to-left one digit at a time and print the result. for sure by using this way he will find a carry for example</p>
<p>1234<br> &nbsp; &nbsp; &nbsp; +<br>5678<br>______<br><br>6912</p>
<p>4+8=2 and carry 1</p>
<p>carry+3+7=carry 1</p>
<p>carry+2+6=9 carry 0</p>
<p>carry+1+5=6&nbsp;</p>
<p>Your job is to create a program that count the number of carry operations.</p>
<h3>Input</h3>
<p>Each line of input contains two unsigned integers less than 10 digits. The last line of input contains ¡®0 0¡¯.</p>
<h3>Output</h3>
<p>For each line of input except the last you should compute and print the number of carry operations that would result from adding the two numbers, in the format shown below.</p>
<h3 style="box-sizing: border-box; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 500; line-height: 1.1; color: #333333; margin-top: 20px; margin-bottom: 10px; font-size: 20px;">Example</h3>
<p>&nbsp;</p>
<pre style="box-sizing: border-box; overflow: auto; font-family: Menlo, Monaco, Consolas, 'Courier New', monospace; font-size: 11px; padding: 10px; margin: 20px 0px; line-height: 1.42857143; color: #333333; word-break: break-all; word-wrap: break-word; border-radius: 3px; background-image: initial; background-attachment: initial; background-size: initial; background-origin: initial; background-clip: initial; background-position: 0px 50%; background-repeat: initial; border: 1px 1px 1px 5px solid #eeeeee #eeeeee #eeeeee #5bc0de;"><span style="box-sizing: border-box;"><span style="box-sizing: border-box; line-height: 15.7142858505249px;"><span style="box-sizing: border-box; font-weight: 700;"><span style="font-family: Menlo, Monaco, Consolas, 'Courier New', monospace; color: #333333;"><span style="font-size: 11px; font-weight: 700; line-height: 15.7142858505249px;">Input:
</span></span><div id="_mcePaste" style="color: #333333; font-family: Menlo, Monaco, Consolas, 'Courier New', monospace; font-size: 11px; font-weight: 700; line-height: 15.7142858505249px; position: absolute; left: -10000px; top: 261px; width: 1px; height: 1px; overflow: hidden;">123 456</div><div id="_mcePaste" style="color: #333333; font-family: Menlo, Monaco, Consolas, 'Courier New', monospace; font-size: 11px; font-weight: 700; line-height: 15.7142858505249px; position: absolute; left: -10000px; top: 261px; width: 1px; height: 1px; overflow: hidden;">555 555</div><div id="_mcePaste" style="color: #333333; font-family: Menlo, Monaco, Consolas, 'Courier New', monospace; font-size: 11px; font-weight: 700; line-height: 15.7142858505249px; position: absolute; left: -10000px; top: 261px; width: 1px; height: 1px; overflow: hidden;">123 594</div><span style="font-family: Menlo, Monaco, Consolas, 'Courier New', monospace; color: #333333;"><span style="font-size: 11px; font-weight: 700; line-height: 15.7142858505249px;">123 456
555 555
123 594<br>0 0<br>
Output:
</span><span style="font-size: 11px; line-height: 15.7142858505249px;">No carry operation.
3 carry operations.
1 carry operation.</span></span></span></span></span></pre>