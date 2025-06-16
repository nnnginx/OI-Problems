<h3>Input</h3>
<p>A Program which has the following format:</p>
<pre>&lt;Program&gt;::=&lt;sentence&gt;&lt;line break&gt;{&lt;sentence&gt;&lt;line break&gt;}
&lt;setence&gt;::=&lt;level&gt;&lt;space&gt;&lt;body&gt;
&lt;body&gt;::=&lt;addition&gt; | &lt;output&gt; | &lt;goto&gt; | &lt;condition&gt; | &lt;end&gt;
&lt;addition&gt;::=&lt;variable&gt;+&lt;integer&gt;
&lt;output&gt;::=&lt;variable&gt;?
&lt;goto&gt;::=GO&lt;space&gt;&lt;level&gt;
&lt;condition&gt;::=IF&lt;space&gt;&lt;variable&gt;=&lt;integer&gt;&lt;space&gt;&lt;goto&gt;
&lt;end&gt;::=END
&lt;variable&gt;::=&lt;character&gt;
&lt;level&gt;::=&lt;integer&gt;
&lt;integer&gt;::=&lt;digit&gt;{&lt;digit&gt;}
&lt;character&gt;::=A|B|C|D|E|F|G|H|I|J|K|L|M|N|O|P|Q|R|S|T|U|V|W|X|Y|Z
&lt;digit&gt;::= 0|1|2|3|4|5|6|7|8|9
&lt;line break&gt;::=(ASCII 10)
&lt;space&gt;::=(ASCII 32)
</pre>
<p>The program runs following the following rules:</p>
<div align="justify">
    <ul>
        <li>
        Program starts from the sentence whose level is minimum, and executed by the level from low to high except that the sentence is&lt;goto&gt;or&lt;condition&gt;.
        </li><li>
        All variables are initialized to 0.
        </li><li>
        &lt;Addition&gt;means&lt;variable&gt;+=&lt;integer&gt;in C++.
        </li><li>
        &lt;output&gt;means write the value of&lt;variable&gt;to the output file(we aren't interesting about the real output file.)
        </li><li>
        &lt;condition&gt;means if and only if the value of the &lt;variable&gt; equals to &lt;integer&gt;, &lt;goto&gt; will be executed, otherwise the next sentence executed is as usual.
        </li><li>
        After&lt;goto&gt;, the next sentence executed is the sentence with level which equals to the level in&lt;goto&gt;.
        </li><li>
        Program terminates by itself when &lt;end&gt; is executed.
        </li><li>
        The numbers during the program is running will fit in a signed 32-bit integer.
        </li><li>
        The number of sentences in the program is not more than 100.
        </li><li>
        The length of each line in the input file is not more than 20.
        </li><li>
        The input is correct.
        </li><li>
        The sentence with the maximum level is always &lt;end&gt;.
        </li><li>
        Any level is not more than 3000.
        </li>
    </ul>
</div>
<p>Input terminate by EOF.</p>
<h3>Output</h3>
<p>Output the number of sentences executed.If the program can not terminate by itself,output -1.</p>
<h3>Example</h3>
<pre><b>Input:</b>
10 A+1
20 IF A=5 GO 60
60 END
30 A+2
40 A?
50 GO 20

<b>Output:</b>
11

<b>Hint:</b>
10-&gt;20-&gt;30-&gt;40-&gt;50-&gt;20-&gt;30-&gt;40-&gt;50-&gt;20-&gt;60
</pre>
<h3>Note</h3>
<p>You may try problem <a href="http://www.spoj.com/problems/ANALYS_T">ANALYS_T</a> first. It's the same problem with this one and its time limit is not so strict, but tests are easier than this problem.</p>

<h3>Log</h3>
<p>The time limit of this problem has been changed from 0.4/0.5 second to 1 second per test on Jun.5, 2008. All the solutions have been rejudged.</p>
<p>Due to compiler changes, the time limit has been shorten to 0.1 second per test.</p>