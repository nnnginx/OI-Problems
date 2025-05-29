<p>Byteotian Interstellar Union (BIU) has recently discovered a new planet in   a nearby galaxy.  The planet is unsuitable for colonisation due to strange   meteor showers, which on the other hand make it an exceptionally interesting   object of study.</p>
<p>The member states of BIU have already placed space stations close to the   planet's orbit.  The stations' goal is to take samples of the rocks flying by.   The BIU Commission has partitioned the orbit into <span><img src="./23369/file/j87ifPuW.png" alt=""></span> sectors, numbered   from <span><img src="./23369/file/5vmV88Iw.png" alt=""></span> to <span><img src="./23369/file/YQrp7tRb.png" alt=""></span>, where the sectors <span><img src="./23369/file/tRetDSdb.png" alt=""></span> and <span><img src="./23369/file/A4wQdqOJ.png" alt=""></span> are adjacent.  In each sector   there is a single space station, belonging to one of the <span><img src="./23369/file/7jaJGfvS.png" alt=""></span> member states.</p>
<p>Each state has declared a number of meteor samples it intends to gather before   the mission ends.  Your task is to determine, for each state, when it can   stop taking samples, based on the meter shower predictions for the years to   come.</p>
<h2>Input</h2>
<p>The first line of the standard input gives two integers, <span><img src="./23369/file/LDRQC5uU.png" alt=""></span> and <span><img src="./23369/file/ehZghlQ6.png" alt=""></span> (<span><img src="./23369/file/YLtGh32n.png" alt=""></span>), separated by a single space, that denote,     respectively, the number of BIU member states and the number of sectors     the orbit has been partitioned into.</p>
<p>In the second line there are <span><img src="./23369/file/TIqBheT6.png" alt=""></span> integers <span><img src="./23369/file/vCEcF6kN.png" alt=""></span> (<span><img src="./23369/file/K5MZXb9D.png" alt=""></span>),     separated by single spaces, that denote the states owning stations in     successive sectors.</p>
<p>In the third line there are <span><img src="./23369/file/OgRhh5Qi.png" alt=""></span> integers <span><img src="./23369/file/9pAaEQj7.png" alt=""></span> (<span><img src="./23369/file/VQ2V2j41.png" alt=""></span>),     separated by single spaces, that denote the numbers of meteor samples that     the successive states intend to gather.</p>
<p>In the fourth line there is a single integer <span><img src="./23369/file/x5UlbsUn.png" alt=""></span> (<span><img src="./23369/file/8oZBhKfe.png" alt=""></span>)     that denotes the number of meteor showers predictions.     The following <span><img src="./23369/file/ZHEiCKvG.png" alt=""></span> lines specify the (predicted) meteor showers     chronologically.  The <span><img src="./23369/file/j4wkrbDT.png" alt=""></span>-th of these lines holds three integers     <span><img src="./23369/file/sFlmn7zh.png" alt=""></span>, <span><img src="./23369/file/0bM4QfzK.png" alt=""></span>, <span><img src="./23369/file/IM9rz25Z.png" alt=""></span> (separated by single spaces), which denote that     a meteor shower is expected in sectors     <span><img src="./23369/file/6Ndhg9Hc.png" alt=""></span> (if <span><img src="./23369/file/gUinvbGr.png" alt=""></span>)     or sectors <span><img src="./23369/file/8UtBtxuq.png" alt=""></span> (if <span><img src="./23369/file/x0qHPe9b.png" alt=""></span>),     which should provide each station in those sectors with <span><img src="./23369/file/kYhoX5o7.png" alt=""></span> meteor samples     (<span><img src="./23369/file/j2zORbZc.png" alt=""></span>).</p>
<h2>Output</h2>
<p>Your program should print <span><img src="./23369/file/5STpbkAT.png" alt=""></span> lines on the standard output.     The <span><img src="./23369/file/oLhJ9qEZ.png" alt=""></span>-th of them should contain a single integer <span><img src="./23369/file/jo4e5n6P.png" alt=""></span>, denoting the number     of shower after which the stations belonging to the <span><img src="./23369/file/KwtBEiQc.png" alt=""></span>-th state are     expected to gather at least <span><img src="./23369/file/L3BFqedS.png" alt=""></span> samples, or the word <tt>NIE</tt> (Polish     for <em>no</em>) if that state is not expected to gather enough samples in the     foreseeable future.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>3 5
1 3 2 1 3
10 5 7
3
4 2 4
1 3 1
3 5 2</pre>
<p>the correct result is:</p>
<pre>3
NIE
1</pre>