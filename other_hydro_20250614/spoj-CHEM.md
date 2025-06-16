<p>The story started some 5¡¯000 years ago in Ancient Egypt, was continued by the Greeks and Arabs, reached France, Europe, and finally conquered the world. The studies on the compositions of waters, the humans¡¯ greed for purified materials, millions of experiments and many brilliant minds made chemistry what it is today: No more the quest of the Philosopher¡¯s stone, but the study of matter and the changes it undergoes.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="../../../content/imuteb:chemistry" alt="" width="390" height="311"></p>
<p>&nbsp;</p>
<p>There remain nevertheless still groups of stout-hearted followers of ancient believes, so-called alchemist. Keeping their research top-secret, they meet once a year for a conference where they share their recent findings. This year¡¯s location is Lausanne and Extremely Purified Fluorescent Liquids (EPFL) is the topic. The idea is that the chemists brew together some new EPFLs. As we speak about state of the art EPFLs, it is necessary that certain chemists put their very specific knowledge together. Thus for a certain EPFL <em>E<sub>1</sub></em>, the presence of chemists <em>C<sub>1</sub></em>, <em>C<sub>2</sub></em> and <em>C<sub>3</sub></em> may be required. For another <em>E<sub>2</sub></em>, chemists <em>C<sub>1</sub></em><sub> </sub>and <em>C<sub>4</sub> </em>might be necessary.</p>
<p>&nbsp;Although chemists are generally very patient people, as their reactions might take long times, they get very impatient if they are to observe experiments in which they are not involved. As an example, chemist <em>C<sub>4</sub></em><sub> </sub>would go crazy if he had to assist to the brewage of <em>E<sub>1</sub></em>. To ensure a pleasant stay in Lausanne to every chemist, you are to arrange their departure and arrival dates so that each chemist is available whenever his knowledge is required, but is not in Lausanne when other EPFLs are created.</p>
<p>To this purpose, you are given a schedule with ones and zeros. Each column stands for one EPFL, each row for one chemist. There is a 1 at position (<em>C<sub>i</sub>,E<sub>i</sub></em>) if chemist<em> C<sub>i</sub></em> is needed for EPFL <em>E<sub>i</sub></em>, and a zero otherwise. Your task boils now down on rearranging the columns in a way that all ones are consecutive in every line. For traditional reasons, the organizers¡¯ EPFL is always brewed first and corresponds to the first column of the input schedule (<em>E<sub>1</sub></em>).</p>
<p><strong>INPUT</strong></p>
<p>The input consists of several test-cases separated by an empty line. Each test-case starts with the number of chemists <em>C</em> (1&lt;=C&lt;=400), followed by the number of EPFLs <em>E</em> (1&lt;=E&lt;=400). Then follow <em>C</em> lines of <em>E </em>characters, ¡®1¡¯ or ¡®0¡¯. You may assume that there exists exactly one order of EPFLs (initiated by <em>E<sub>1</sub></em>) that meets the above constraints. Input terminates on a test-case with <em>C=E=0</em>, which must not be processed.</p>
<p>&nbsp;</p>
<p><strong>OUTPUT</strong></p>
<p>Print each output on a line by itself, which holds <em>E</em> numbers, corresponding to the initial position in the planning, arranged such that all chemists are available when necessary and away from Lausanne otherwise. (the first number must always be 1 as a tribute to the host).</p>
<p>&nbsp;</p>
<p><strong>SAMPLE INPUT</strong></p>
<p>6 5</p>
<p>00010</p>
<p>01000</p>
<p>10101</p>
<p>10100</p>
<p>00011</p>
<p>00101</p>
<p>&nbsp;</p>
<p>0 0</p>
<p>&nbsp;</p>
<p><span style="font-family: courier new,courier;">&nbsp;</span></p>
<p><strong>SAMPLE OUTPUT</strong></p>
<p>1 3 5 4 2</p>
<p>&nbsp;</p>