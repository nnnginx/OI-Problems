<p><strong>[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2016 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at&nbsp;<a href="http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf</a>&nbsp;]</strong></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Finishing your studies in a university is not only a matter of studying and learning. To obtain</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">that prized degree, each student has to prove that he has learned, and in order to do that he</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">needs to pass $N$ subjects. However, it is often also necessary to abide by uncountable and deliberately</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">complicated regulatory labyrinths.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">At the \emph{Institute With Few Correlations} (IWFC) there are antiquated norms which forbid students</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">from passing some subjects without having first passed certain other subjects. The latter are called</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">``correlation'' subjects for the first ones. Each subject may have one or more correlation subjects, but there</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">are no cyclic correlations, so that it is always possible to obtain the desired degree.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Gabina is a student of Happiness Sciences, and fortunately her professors are very understanding people.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">They therefore allow her to pass her subjects without actually having passed their correlation subjects before.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The problem with this is that IWFC's electronic system can only register a subject as being passed abiding</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">by the correlation rules. Thus, a subject will be registered in the system if and only if it was passed and all its correlation</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">subjects are also already registered.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Seeing her progress keeps Gabina motivated, and helps her to push forward with her studies. For this reason, each</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">time she passes a subject she checks the electronic system to see how many subjects have been registered in it.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sometimes she sees the number has not changed, which happens whenever the subject she just passed didn't have all</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">its correlation subjects registered in the system. In other cases, she receives the delightful news that the number</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">of registered subjects has increased. Moreover, it may happen that this increase was in more than one, which happens</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">whenever the subject she just passed could be registered, and doing so unlocked the registration of a series of&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">subjects passed beforehand.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Gabina has already planned the order in which she will pass all the subjects for her degree. She would now like to know</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">the number of subjects which will be registered in the electronic system after she passes each one of them. Your task is&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">to write a program to help Gabina predict this, so that she can joyfully finish her Happiness Sciences studies.</div>
<p>Finishing your studies in a university is not only a matter of studying and learning. To obtain that prized degree, each student has to prove that he has learned, and in order to do that he needs to pass <strong>N</strong>&nbsp;subjects. However, it is often also necessary to abide by uncountable and deliberately complicated regulatory labyrinths.</p>
<p>At the <em>Institute With Few Correlations</em>&nbsp;(IWFC) there are antiquated norms which forbid students from passing some subjects without having first passed certain other subjects. The latter are called "correlation" subjects for the first ones. Each subject may have one or more correlation subjects, but there are no cyclic correlations, so that it is always possible to obtain the desired degree.</p>
<p>Gabina is a student of Happiness Sciences, and fortunately her professors are very understanding people. They therefore allow her to pass her subjects without actually having passed their correlation subjects before. The problem with this is that IWFC's electronic system can only register a subject as being passed abiding by the correlation rules. Thus, a subject will be registered in the system if and only if it was passed and all its correlation subjects are also already registered.</p>
<p>Seeing her progress keeps Gabina motivated, and helps her to push forward with her studies. For this reason, each time she passes a subject she checks the electronic system to see how many subjects have been registered in it. Sometimes she sees the number has not changed, which happens whenever the subject she just passed didn't have all its correlation subjects registered in the system. In other cases, she receives the delightful news that the number of registered subjects has increased. Moreover, it may happen that this increase was in more than one, which happens whenever the subject she just passed could be registered, and doing so unlocked the registration of a series of subjects passed beforehand.</p>
<p>Gabina has already planned the order in which she will pass all the subjects for her degree. She would now like to know the number of subjects which will be registered in the electronic system after she passes each one of them. Your task is to write a program to help Gabina predict this, so that she can joyfully finish her Happiness Sciences studies.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. The first line contains two integer numbers <strong>N</strong>&nbsp;and <strong>M</strong>, representing the number of subjects in her degree and the number of correlation relations between pairs of subjects, respectively (<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;N,M ¡Ü&nbsp;5 ¡Á&nbsp;10<sup>4</sup></strong>). The subjects are numbered from <strong>1</strong>&nbsp;to <strong>N</strong>. Each of the following <strong>M</strong>&nbsp;lines contains two integer numbers <strong>A</strong>&nbsp;and <strong>B</strong>, indicating that subject <strong>A</strong>&nbsp;is a correlation subject for subject <strong>B</strong>&nbsp;(<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;A, B&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;N</strong>&nbsp;with <strong>A ¡Ù&nbsp;B</strong>). This means that subject <strong>A</strong>&nbsp;must be registered in the electronic system before subject <strong>B</strong>&nbsp;can be registered. There are no repeated or cyclic correlation relations in the input. The last line contains <strong>N</strong>&nbsp;integer numbers <strong>P<sub>1</sub>, P<sub>2</sub>, ..., P<sub>N</sub></strong>, representing the subjects in the order Gabina will pass them (<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;P<sub>i</sub>&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;N</strong>&nbsp;for <strong>i = 1, ..., N</strong>, with <strong>P<sub>i</sub> ¡Ù&nbsp;P<sub>j</sub></strong>&nbsp;for <strong>i ¡Ù&nbsp;j</strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print <strong>N</strong>&nbsp;lines, each with a single integer number. The number printed in the <strong>i</strong>-th line represents the number of subjects registered in the electronic system immediately after Gabina passes the <strong>i</strong>-th subject for her degree in the order giver in the input.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">3 2
1 2
2 3
1 2 3
3 2
1 2
2 3
3 2 1
4 4
1 2
2 3
4 3
1 4
2 3 1 4</span>

<strong>Output:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">1
2
3
0
0
3
0
0
2
4</span></pre>