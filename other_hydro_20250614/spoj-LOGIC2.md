<p>Some day in 2003 in Byteland began calm and quietly as any other day. Some people went to work, some to school, some to store to buy food. Drivers were traditionally stucked in traffic jams, drinking coffee and reading morning newspaper. Suddenly the regularity of this day was disturbed by huge explosion."They blew up the embassy of Bajtocja!!!"  somebody cried. Everybody began to run away in panic. </p>
<p>Police works pretty good in Byteland and first radiocars appeared near the embassy only few seconds after the explosion. All the people near the embassy were detained. Only one of the people is the organizer of the explosion, the others could by just occasional witnesses. It is known, among these M(1&lt;=M&lt;=11) people, N(1&lt;=N&lt;=M) people always lie because they want to make the work of police more difficult, the others always tell the truth.</p>
<p>All these people say P(1&lt;=P&lt;=30) sentences in total.All the useful sentences are in one of the 4 forms below, all the other sentences are useless and you can ignore them.</p>
<div align="justify">
       <ul>
               <li>
               I am guilty.
               </li><li>
               I am not guilty.
               </li><li>
               <i>Somebody</i> is guilty.
               </li><li>
               <i>Somebody</i> is not guilty.
               </li><li>
               Today is <i>Someday</i>.
               </li>
       </ul>
</div>
<p>Among these sentences, <i>Somebody</i> is a name of one of these M people, and <i>Someday</i> is Monday, Tuesday, Wednesday, Thursday, Friday, Saturday or Sunday.</p>
<p>Your task is to help the police to find out the only one organizer of the explosion.</p>
<h3>Input</h3>
<p>Multiple test cases. For each test case: </p>
<p>The first line contains three integers M, N and P. M lines follow, each contains a name of one of the people.All names contain only capital Latin letters and no whitespaces.P lines come next, each contains no more than 250 characters, the speaker and his/her speech. See the example.</p>
<p>You can assume that there's no whitespace at the start and the end of a line, and there are no two consecutive spaces in the input.</p>
<p>Input terminate by EOF.</p>
<h3>Output</h3>
<p>The name of the organizer if you can determine, or <i>Cannot Determine</i> if you find more than one person is possible, or <i>Impossible</i> if you find the situation is contradictory.</p>
<h3>Example</h3>
<pre><b>Input:</b>
3 1 5
MIKE
CHARLES
KATE
MIKE: I am guilty.
MIKE: Today is Sunday.
CHARLES: MIKE is guilty.
KATE: I am guilty.
KATE: How are you??

<b>Output:</b>
MIKE
</pre>