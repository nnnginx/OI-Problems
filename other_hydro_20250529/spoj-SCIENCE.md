<p>Welcome, ladies and gentlemen, to Aperture Science. Astronauts, war heroes, Olympians -- you're here because we want the best, and you are it. That said it's time to make some science.</p>
<p>Now I want each of you to stand on one of these buttons. Well done, we're making great progress here. Now let's do it again. Oh come on, don't stand on the same button. Move people! No, no, that button's only for the astronauts, you know who you are. What?! You say you can't do everything I ask. Ok let's start over. You there, the Olympian, figure out how many times we can do this. And make it quick, we have a lot more science to get through.</p>
<h3>Input</h3>
<p>The first line will contain N (2 ¡Ü N ¡Ü 200) giving the number of people (and the number of buttons) in the experiment. The next N lines will contain N characters each. If the jth character of the ith line is 'Y' it indicates that the ith person can stand on the jth button (it is 'N' otherwise). The last line of input will be a 0.</p>
<h3>Output</h3>
<p>If it is impossible to get everyone on the buttons at once output "NO SCIENCE" (quotes for clarity). Otherwise first output K, the maximum number of times everyone can be standing on buttons such that nobody stands on the same button more than once. After that output K lines. Each line should contain N integers separated by a space where the ith integer describes who is on the ith button. All of the lines should be valid and none of them should put the same person on the same button.&nbsp; If there are multiple solutions, output any of them.</p>
<h3>Examples</h3>
<pre><strong>Input:</strong>
<br>3<br>YYY<br>NYY<br>YNY

<strong>Output:</strong>
<br>2<br>1 2 3<br>3 1 2<br><strong><br>Input:</strong>
<br>2<br>YN<br>YN
<strong><br>Output:</strong>
<br>NO SCIENCE</pre>