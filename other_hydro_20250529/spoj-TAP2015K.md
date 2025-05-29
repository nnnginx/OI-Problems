<p><span style="font-weight: bold;">[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2015 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at </span><a style="font-weight: bold;" href="http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf</a><span style="font-weight: bold;"> ]</span></p>
<p>Kenya is the birthplace of some of the best long-distance runners of all times. Indeed, eight of the most recent ten best times in the traditional 41.195 km of the marathon have been set by runners from that country. Dennis Kimetto, Wilson Kipsang and Eliud Kipchoge are three such runners, and they want to beat their discipline's world record once more tomorrow September 27, when they compete in the 42<sup>nd</sup> edition of the Berlin Marathon.</p>
<p>Kimetto, Kipsang and Kipchoge are good friends, and they like to train together running by the Tana river in order to appreciate the beautiful trees that grow there. There are <strong>N</strong> trees by the river, which we will number from <strong>1</strong> to <strong>N</strong>. The <strong>i</strong>-th tree is of the species <strong>S<sub>i</sub></strong>&nbsp;and stands at a distance of <strong>i</strong> meters from the mouth of the river. Our three runners are especially motivated by the sight of many trees of different species. For this reason, each training day they choose a tree with number <strong>K</strong> from <strong>1</strong> to <strong>N</strong>, and then run from the <strong>K</strong>-th tree following the river, <em>i.e.</em> in the direction of trees <strong>K-1</strong>, <strong>K-2</strong> and so on, stopping only when they see a tree of some species they have already seen that day, or when they reach the mouth of the river, whichever comes first.</p>
<p>For example, if there are <strong>N = 4</strong> trees of species <strong>S<sub>1</sub>&nbsp;= 1</strong>, <strong>S<sub>2</sub>&nbsp;= 2</strong>, <strong>S<sub>3</sub>&nbsp;= 1</strong> and <strong>S<sub>4</sub>&nbsp;= 3</strong>, when they choose <strong>K = 4</strong> the training consists in running <strong>3</strong> meters, from tree number <strong>4</strong> up to tree number <strong>1</strong> (where they stop because this tree is of the same species as tree number <strong>3</strong>). However, if they chose <strong>K = 2</strong> they would run two meters up to the mouth of the river, where they would stop even without having seen two trees of the same species as they went.</p>
<p>Long-distance running requires decades of training, and in this time it is common for some trees to fall during storms. When this happens, the fallen tree is immediately replaced by another one, not necessarily of the same species. Kimetto, Kipsang and Kipchoge keep a diary where they take note of all the information relevant to their training. In particular, they know the species of all trees, and which number they chose to start running each day of training. Can you help them calculate how much they ran each training day?</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains two integers <strong>N</strong> and <strong>R</strong>, representing respectively the number of trees by the river and the number of entries in the training diary (<strong>1 ¡Ü N, R ¡Ü 5 ¡Á&nbsp;10<sup>4</sup></strong>). The second line contains <strong>N</strong> integers <strong>S<sub>i</sub></strong>&nbsp;indicating the species of the <strong>i</strong>-th tree when the training began (<strong>1 ¡Ü S<sub>i</sub>&nbsp;¡Ü 10<sup>6</sup></strong> for <strong>i = 1, 2, ..., N</strong>). Each of the following <strong>R</strong> lines contains the description of an entry in the training diary, in chronological order. This description starts with a character which can be a <strong>'<span style="font-family: 'courier new', courier;">C</span>'</strong> if the entry corresponds to a fallen tree or an <strong>'<span style="font-family: 'courier new', courier;">E</span>'</strong> if it corresponds to a training day. The entries for fallen trees contain two integers <strong>K</strong> and <strong>S</strong> after the <strong>'<span style="font-family: 'courier new', courier;">C</span>'</strong>, indicating that the <strong>K</strong>-th tree fell and was replaced by another tree of species <strong>S</strong> (<strong>1 ¡Ü K ¡Ü N</strong> and <strong>1 ¡Ü S ¡Ü 10<sup>6</sup></strong>). The entries for training days contain an integer <strong>K</strong> after the <strong>'<span style="font-family: 'courier new', courier;">E</span>'</strong>, indicating that the runners began a training day by running from the <strong>K</strong>-th tree (<strong>1 ¡Ü K ¡Ü N</strong>). There will always be at least one entry for a training day in each test case.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print one line for each entry corresponding to a training day, indicating the number of meters Kimetto, Kipsang and Kipchoge ran during that day.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4 2
1 2 1 3
E 4
E 2
10 10
1 2 3 4 5 6 7 8 9 10
E 1
E 2
E 3
E 4
E 5
E 6
E 7
E 8
E 9
E 10
5 7
1 2 3 4 5
E 3
E 5
C 3 1
E 4
C 2 5
E 3
E 5</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">3
2
1
2
3
4
5
6
7
8
9
10
3
5
3
2
3</span><span style="white-space: normal;">
</span></pre>