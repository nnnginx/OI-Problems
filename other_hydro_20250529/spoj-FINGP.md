<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">professor Emad Eldin one of the best people in pattern recognation , he asked his students to create a program to check if a spicial pattern belongs to fingerprints of someone or not.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">he said that we can consider that a computer reads the special pattern and the fingerprint as strings , and we can say that the fingerprint belongs to special pattern if&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">the last substring of the fingerprints string is the same as special pattern string.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Your task is to help professor Emad students.</div>
<p>professor Emad Eldin one of the best people in pattern recognation , he asked his students to create a program to check if a special pattern belongs to fingerprints of someone or not.</p>
<p>he said that we can consider that a computer reads the special pattern and the fingerprints as strings , and we can say that the special pattern belongs to the fingerprint if the last substring of the fingerprint string is the same as the special pattern string.</p>
<p>Your task is to help professor Emad students.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p><span style="font-size: small;">The first line of the input contains special pattern string S<span class="tex-span" style="color: #222222; line-height: 19.6000003814697px;">(1 ≤ |<em>S</em>| ≤ 50)</span>. second line will be a single integer N, the number of fingerprints (1 ≤ N ≤ 10).N lines follow, each line contains fingerprint string F<span class="tex-span" style="color: #222222; line-height: 19.6000003814697px;">(1 ≤ |<em>F</em>| ≤ 50)</span>.</span></p>
<h3>Output</h3>
<p>For each test case, print an integer K, the number of fingerprints strings that spicial pattern string belongs to it. Followed by K lines, each contains the fingerprint string that the special pattern string belongs to it. You should print the fingerprint strings in a lexicographical order. If there is no fingerprint belongs to the special pattern , print "Wrong fingerprints!" instead.</p>
<h3 style="box-sizing: border-box; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; font-weight: 500; line-height: 1.1; color: #333333; margin-top: 20px; margin-bottom: 10px; font-size: 20px;"><span style="font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; color: #333333;"><span style="font-size: 20px; font-weight: 500; line-height: 1.1;"><br>Examples</span></span><br><br>
<pre style="box-sizing: border-box; overflow: auto; font-family: Menlo, Monaco, Consolas, 'Courier New', monospace; font-size: 11px; padding: 10px; margin: 20px 0px; line-height: 1.42857143; color: #333333; word-break: break-all; word-wrap: break-word; border-width: 1px 1px 1px 5px; border-style: solid; border-color: #eeeeee #eeeeee #eeeeee #5bc0de; border-radius: 3px; background-image: initial; background-attachment: initial; background-size: initial; background-origin: initial; background-clip: initial; background-position: 0px 50%; background-repeat: initial;"><span style="box-sizing: border-box;"><span style="box-sizing: border-box; line-height: 15.7142858505249px;"><span style="box-sizing: border-box; font-weight: 700;">Input:
On
5
Pattern recognatiOn
CommOn patterN
game
organizatiOn
lion
<br>Output:<br>2
Pattern recognatiOn
organizatiOn</span></span></span></pre>
<pre style="box-sizing: border-box; overflow: auto; font-family: Menlo, Monaco, Consolas, 'Courier New', monospace; font-size: 11px; padding: 10px; margin: 20px 0px; line-height: 1.42857143; color: #333333; word-break: break-all; word-wrap: break-word; border-width: 1px 1px 1px 5px; border-style: solid; border-color: #eeeeee #eeeeee #eeeeee #5bc0de; border-radius: 3px; background-image: initial; background-attachment: initial; background-size: initial; background-origin: initial; background-clip: initial; background-position: 0px 50%; background-repeat: initial;"><span style="font-family: Menlo, Monaco, Consolas, 'Courier New', monospace; color: #333333;"><span style="font-size: 11px; line-height: 15.7142858505249px;">Input:
Ze<br>2
Fingerprint
pattern design<br>
Output:
Wrong fingerprints!</span></span></pre>
<p style="margin: 1.5em 0px 0px; padding: 0px; font-size: 14px; line-height: 1.4em; color: #222222; font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;">Notes<br><br>- String&nbsp;<span class="tex-span" style="font-size: 17.5px; font-family: 'times new roman', sans-serif;"><em>S</em></span>&nbsp;contains upper-case English letters ('A' - 'Z') and lower-case English letters ('a' - 'z') only.</p>
<p style="margin: 1.5em 0px 0px; padding: 0px; font-size: 14px; line-height: 1.4em; color: #222222; font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;">- All other strings in the input contains upper-case English letters ('A' - 'Z'), lower-case English letters ('a' - 'z') and spaces (' ') only.</p>
<p style="margin: 1.5em 0px 0px; padding: 0px; font-size: 14px; line-height: 1.4em; color: #222222; font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;">- All strings are case sensitive ('A' is not equal to 'a').</p>
<p style="margin: 1.5em 0px 0px; padding: 0px; font-size: 14px; line-height: 1.4em; color: #222222; font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;">-Lexicographical order is defined in following way. When we compare s and t, first we find the leftmost position with differing characters: si ≠ ti. If there is no such position (i. e. s is a prefix of t or vice versa) the shortest string is less. Otherwise, we compare characters si and ti according to their order in alphabet.</p>
</h3>