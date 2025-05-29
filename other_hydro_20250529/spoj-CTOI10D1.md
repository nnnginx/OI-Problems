<h1><strong><span>The MP3 Player</span></strong></h1>
<p>Georg's new MP3 player has many interesting features, one of them  being the key lock. All the keys are locked after more than <span><em>T</em></span> seconds of inactivity. After the key lock is engaged, no key performs its original function, but if any key is pressed, the  key lock is disengaged.</p>
<p>For example, assume that <span><em>T</em> = 5</span> and the player is currently locked. Georg presses the key <span><em>A</em></span>, waits for 3  seconds, presses the key <span><em>B</em></span>, waits for 5 seconds, presses <span><em>C</em></span>,  waits for 6 seconds, and presses <span><em>D</em></span>. In this case only the keys <span><em>B</em></span> and <span><em>C</em></span> perform their regular functions. Note that the keys became locked between <span><em>C</em></span> and <span><em>D</em></span> was pressed.</p>
<p>Sound level of the MP3 player is controlled by the <tt>+</tt> and <tt>-</tt> keys, increasing and decreasing volume by <span>1</span> unit respectively. The sound level is an integer between <span>0</span> and  <span><em>V</em><sub><em>m</em><em>a</em><em>x</em></sub></span>.  Pressing the <tt>+</tt> key at volume <span><em>V</em><sub><em>m</em><em>a</em><em>x</em></sub></span> or pressing the <tt>-</tt> key at volume <span>0</span> leaves the volume unchanged.</p>
<p><a id="Task_specification" name="Task_specification"></a></p>
<h2><strong><span>Task specification</span></strong></h2>
<p>Georg does not know the value of <span><em>T</em></span>.  He wanted to find it by an experiment.  Starting with a locked keyboard, he pressed a sequence of <span><em>N</em></span> <tt>+</tt> and <tt>-</tt> keys. At the end of the experiment Georg read the final volume from the  player's display.  Unfortunately, he forgot to note the volume before his first keypress. For the purpose of this task, the unknown initial volume will be denoted  <span><em>V</em><sub>1</sub></span> and the known final volume will be denoted <span><em>V</em><sub>2</sub></span>.</p>
<p>You are given the value <span><em>V</em><sub>2</sub></span> and a list of keystrokes in the order in which Georg made them. For each key, you are given the type of the key (<tt>+</tt> or <tt>-</tt>) and the number of seconds from the beginning of the experiment to the  moment when the key was pressed. The task is to find the largest possible <strong>integer</strong> value  of <span><em>T</em></span> which is consistent with the outcome of the experiment.</p>
<p><a id="Input_specification" name="Input_specification"></a></p>
<h2><strong><span>Input specification</span></strong></h2>
<p>The first line of the input contains three space-separated integers <span><em>N</em></span>, <span><em>V</em><sub><em>m</em><em>a</em><em>x</em></sub></span> and  <span><em>V</em><sub>2</sub></span> (<img src="./22017/file/ZdodCiyM.png" alt="0 \leq V_2 \leq V_{max}">).  Each of the next <span><em>N</em></span> lines contains a  description  of one key in the sequence: a character <tt>+</tt> or <tt>-</tt>, a space and an integer <span><em>C</em><sub><em>i</em></sub></span> (<img src="./22017/file/xqbHYmik.png" alt="0 \leq C_i \leq 2\cdot 10^9">),  the number of seconds from the beginning of the experiment. You may  assume that the keypresses are in sorted order and that all times are distinct (i.e., <span><em>C</em><sub><em>i</em></sub> &lt; <em>C</em><sub><em>i</em> + 1</sub></span> for all <img src="./22017/file/PbYMOglE.png" alt="1 \leq i < N">).</p>
<p><a id="Constraints" name="Constraints"></a></p>
<h2><strong><span>Constraints</span></strong></h2>
<p>You may assume that <img src="./22017/file/5phh5ny9.png" alt="2 \leq N \leq 100\,000"> and <img src="./22017/file/PBVMybNZ.png" alt="2 \leq V_{max} \leq 5\,000">.</p>
<p>In test cases worth 40 points <img src="./22017/file/mJqnCZgv.png" alt="N \leq  4\,000">.</p>
<p>In test cases worth 70 points <img src="./22017/file/ncKtjdqj.png" alt="N \cdot  V_{max} \leq 400\,000">.</p>
<p><a id="Output_specification" name="Output_specification"></a></p>
<h2><strong><span>Output specification</span></strong></h2>
<p>If <span><em>T</em></span> can be arbitrarily large,  output a single line containing the word "<tt>infinity</tt>" (quotes for clarity).</p>
<p>Otherwise, output a single line containing two integers <span><em>T</em></span> and <span><em>V</em><sub>1</sub></span> separated by a single space.</p>
<p>The values must be such that carrying out the experiment with  locking time <span><em>T</em></span> starting at volume   <span><em>V</em><sub>1</sub></span> gives the final volume  <span><em>V</em><sub>2</sub></span>. If there are multiple possible answers, output the one with the largest <span><em>T</em></span>; if there are still multiple possible answers, output the one with the largest <span><em>V</em><sub>1</sub></span>.</p>
<p>(Note that at least one solution always exists: for <span><em>T</em> = 0</span> none of the keys performs its  action, so it suffices to take <span><em>V</em><sub>1</sub> = <em>V</em><sub>2</sub></span>.)</p>
<p><a id="Examples" name="Examples"></a></p>
<h2><strong><span>Examples</span></strong></h2>
<p><strong><strong>input:</strong></strong></p>
<pre>6 4 3<br>- 0<br>+ 8<br>+ 9<br>+ 13<br>- 19<br>- 24<br></pre>
<p><strong><strong>output:</strong></strong></p>
<pre>5 4<br></pre>
<p><em>For <span><em>T</em> = 5</span> the keys perform the  following actions: unlock, unlock, <tt>+</tt>, <tt>+</tt>, unlock, <tt>-</tt>.</em></p>
<p><em>For any <img src="./22017/file/pmCbtUmh.png" alt="V_1\in\{2,3,4\}"> we would get <span><em>V</em><sub>2</sub> = 3</span>. Note  that the output contains the largest possible <span><em>V</em><sub>1</sub></span>.</em></p>
<p><em>For <img src="./22017/file/JNUrdixn.png" alt="T\geq 6"> the last two keystrokes will both be active, hence it will be impossible  to</em> have <span><em>V</em><sub>2</sub> = 3</span>.</p>
<p><br> <strong><strong>input:</strong></strong></p>
<pre>3 10 10<br>+ 1<br>+ 2<br>+ 47<br></pre>
<p><strong><strong>output:</strong></strong></p>
<pre>infinity<br></pre>
<p><em>If <span><em>V</em><sub>1</sub> = 10</span> then for  any <span><em>T</em></span> we'll have <span><em>V</em><sub>2</sub> = 10</span>.</em></p>