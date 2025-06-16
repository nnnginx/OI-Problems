<p>In a secret forest, there are many trolls. They are intelligent and most of them even knows programming languages C or PASCAL. They have written many programs. With their super computers, their programs will run for a very short time and they can get the correct answer. Being an excellent programmer, you can even come up with the answer without computers!!!</p>
<h3>Input</h3>
<p>There's no real input file. The four programs can be downloaded <a href="http://www.spoj.com/content/john_jones:trolls.zip">here</a>.
</p><h3>Output</h3>
<p>For <b>program1.txt</b> and <b>program2.txt</b> in the zip file:</p>
<p>Your output should contain a single integer denoting the number of "*" the program will output.</p>
<p>For <b>program3.txt</b> and <b>program4.txt</b> in the zip file:</p>
<p>Your output should contain a single integer denoting the number the program will output.</p>
<p>You can merge the 4 output lines together to get the real output file and submit it.</p>
<h3>Example</h3>
<p>If <b>program1.txt</b> is </p>
<pre>var i:integer;
begin
  for i:=2 to 8 do write('*');
end.

#include &lt;stdio.h&gt;
void main() {
  int i;
  for(i=2; i&lt;=8; i++) printf("*");
}
</pre>
<p>The corresponding line should be:</p>
<pre>7
</pre>
<p>If <b>program3.txt</b> is </p>
<pre>var a, i: integer;

begin
  a := 0;
  for i:= 1 to 9 do
    a := a * 10 + i;
  writeln(a);
end.


#include &lt;stdio.h&gt;

void main() {
  int i, a;
  a = 0;
  for(i=1; i&lt;=9; i++)
    a = a * 10 + i;
  printf("%d\n", a);
}
</pre>
<p>The correspoding line should be</p>
<pre>123456789
</pre>
<h3>Note</h3>
<p>The numbers fit into the type "int" in C program or "integer" in PASCAL program in the zip file can be arbitrarily large because the computers used by trolls are <b>super computers</b>.</p>