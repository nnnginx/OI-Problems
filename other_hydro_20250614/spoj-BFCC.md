<p>The citizens of Palinopolis are very fond of arguments. Whenever two Palinopolitans meet up, whether it be to negotiate over territorial boundaries or buy a pet, custom requires them to take up contrary positions and argue for at least five minutes, then finally depart in frustrated disagreement. The most gifted arguers often pursue careers at prestigious argument firms, but in order to secure a job they must first survive a stringent regime of exams followed by a highly competitive hiring process. In the first round of hiring, each applicant must face off against the head of the firm for ten hours without agreeing on a single point. In the second round, the remaining applicants face each other. These applicants are conveniently numbered from 1 to <strong>N</strong>, and a topic is chosen that allows <strong>N</strong> mutually opposing viewpoints <strong>V</strong><sub>1</sub>, <strong>V</strong><sub>2</sub>, ..., <strong>V</strong><sub><strong>N</strong></sub> to be assigned to them respectively. Next, pairs of applicants are successively chosen and locked in a small, humid room to argue their respective viewpoints until one of them becomes conciliatory, gives up, or passes out. The loser is not eliminated outright but must take on the viewpoint of the victor in subsequent matches. Additionally, anyone else who is currently assigned the losing opponent's viewpoint must change his viewpoint to the victor's. It may happen that some pairs are chosen such that each opponent represents the same viewpoint. This is in fact no problem at all, since any Palinopolitan worth his salt is perfectly capable of conducting a heated argument with someone who is expressing the exact same views. No applicant is ever asked to argue against himself, however, as that would just be silly.</p>

<p>The final selection of applicants is based on many complex factors, including percentage of matches won, number of hours passed out, and whether or not the judge has had a good lunch that day. As a member of the oversight committee, part of your job is to analyse the matches and provide relevant figures and statistics to your superiors. One crucial bit of information (according to your boss) is how many viewpoints survived the process, and which groups of applicants share the same assigned viewpoint. This would normally be quite an easy task for you to solve, except that today your boss is in a bad mood and would like to punish you by making you solve it in a strange, primitive programming language that he just read about on the internet when he was supposed to be working.</p>

<p><strong>Note:</strong> You can use any programming language you want, as long as it is brainf**k.</p>

<h3>Input</h3>

<p>First an integer <strong>T</strong> (1 �� <strong>T</strong> �� 1000), followed by <strong>T</strong> tests. Each test starts with two integers <strong>N</strong> (1 �� <strong>N</strong> �� 50) and <strong>M</strong> on a line, the number of applicants and the number of matches respectively. Then in the following <strong>M</strong> lines are given pairs of integers <strong>u</strong> and <strong>v</strong> in the range [1..<strong>N</strong>], indicating that applicants <strong>u</strong> and <strong>v</strong> face each other in a match. Finally, every case (including the last) ends with a blank line.

</p><h3>Output</h3>

<p>For each case, first print out <strong>K</strong>, the number of distinct viewpoints surviving at the end of all matches, and then print out each group of applicants sharing a common viewpoint. Each group must be sorted internally, and the groups must also be sorted with respect to each other, using the usual definitions for sorting lists (lexicographically).</p>

<h3>Example</h3>

<p><strong>Input:</strong></p>
<pre>2
3 1
2 3

9 7
4 1
8 2
4 6
5 1
5 7
6 1
5 6

</pre>

<p><strong>Output:</strong></p>
<pre>2
1
2 3
4
1 4 5 6 7
2 8
3
9
</pre>

<h3>Additional Info</h3>

<p>The input is generated as follows: <strong>N</strong> is chosen uniform randomly in the range, then <strong>K</strong> is chosen uniform randomly in [1..<strong>N</strong>] and a minimal number of edges is chosen randomly to yield <strong>K</strong>, then the extra edges (that do not change <strong>K</strong>) are chosen randomly with probability <strong>p</strong>, where <strong>p</strong> is uniform random in [0,1]. Duplicate edges do not appear.</p>

<p>There are two data sets, one with <strong>T</strong>=1000 and the other with <strong>T</strong>=500. My solution at the time of publication has 1192 bytes (not golfed) and runs in 9.37s with 2.3M memory footprint.</p>

<p>The custom judge reports your source code length in parentheses after the judge result (when available at the time of judge termination). Only valid BF commands are counted. Also, if you don't get AC, you will be told on which data set you first failed (0-indexed). (The master judge is the same as <a href="http://www.spoj.com/problems/BFPRMCYC/">BFPRMCYC</a>, and the test case judge is the same as <a href="http://www.spoj.com/problems/BFBINADD/">BFBINADD</a>.)</p>