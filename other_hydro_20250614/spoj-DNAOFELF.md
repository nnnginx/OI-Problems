<div>
<p>Everyone knows that Santa's Elfs are non-gendered and reproduce  by magic. Every time a new Elf is needed, two other Elfs come together,  build a snowman, put a hair of each of them on him and then use their  magical powers to give life to the snowman who becomes an Elf. This Elf  always inherits the magical powers of its creators, unless both creators  possess the same type of power, so the new Elf does not inherit such  power because there is a magical overhead. Elfs, too, never create other  elves without magical powers.</p>
<p>Because it was so easy to create new Elfs, Santa realized that  his subordinates were creating many new helpers, not thinking about the  consequences. Simply to lessen your workloads. So he decided to forbid  the creation of new Elfs who already had the same set of powers as any  existing Elf, as this would be redundant given that a single Elf with  that set of powers is more than enough for the function that is  designated. In addition there may already be more than one Elf of that  type because it was created before Good Old Man vetoed the creations.</p>
<p>Now the little magical beings live a dilemma: Given the  information of all types of powers that each Elf has, what is the  maximum number of new Elfs that can still be created?</p>
</div>
<h3>Input</h3>
<div>
<p>The first line of the entry contains an integer <strong>T</strong> corresponding to the number of test cases that follow. The first line of a test case contains an integer <strong>N</strong> (1 ¡Ü <strong>N</strong> ¡Ü 10<sup>5</sup>) representing the number of Elfs currently in the Santa factory. The following are <strong>N</strong> lines each containing a sequence of max. 64 characters <strong>C<sub>i</sub></strong>. <strong>C<sub>i</sub></strong> is always a lowercase or uppercase letter of the English alphabet or a  digit from 0 to 9 and represents a type of magic power. Lowercase  letters represent types of magic power distint than uppercase letters.</p>
</div>
<h3>Output</h3>
<p>The output consists of one line per test case containing the maximum  number of Elfs that can still be created without contradicting Santa's  ban</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>3
</p><p>2
</p><p>xz
</p><p>yx
</p><p>3
</p><p>xz
</p><p>yx
</p><p>zy
</p>5
<p>xazt
</p><p>ctz
</p><p>cax
</p><p>xz
</p><p>at</p>

<strong>Output:</strong>
<p>1
</p><p>0
</p><p>2</p></pre>