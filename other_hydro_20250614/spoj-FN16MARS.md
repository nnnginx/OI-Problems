<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Real-time software in the Mars Pathfinder spacecraft     suffered from an issue known as priority inversion. One     technique to address this issue is to use the Priority Ceiling     Protocol.</p>
<p>In this problem, you will simulate the execution of multiple     tasks according to this protocol. The tasks share a collection     of resources, each of which can be used by only one task at a     time. To ensure this, resources must be locked before use and     unlocked after use. Each task is defined by a start time, a     unique <em>base priority</em>, and a sequence of instructions.     Each task also has a <em>current priority</em>, which may     change during execution. Instructions come in three types:</p>
<ul class="itemize">
<li>
<p><em>compute</em> ¨C perform a computation for         one&nbsp;microsecond</p>
</li>
<li>
<p><em>lock $k$</em> ¨C         lock resource $k$         (which takes no processor time)</p>
</li>
<li>
<p><em>unlock $k$</em> ¨C unlock resource $k$         (which takes no processor time)</p>
</li>
</ul>
<p>After locking a resource, a task is said to <em>own</em> the     resource until the task unlocks it. A task will unlock only the     owned resource it most recently locked, will not lock a     resource it already owns, and will complete with no owned     resources.</p>
<p>Each resource has a fixed <em>priority ceiling</em>, which     is the highest base priority of any task that contains an     instruction to lock that resource.</p>
<p>There is a single processor that executes the tasks. When     the processor starts, it initializes its clock to zero and then     runs an infinite loop with the following steps:</p>
<dl class="description"> <dt>Step 1.</dt> <dd>
<p>Identify <em>running</em> tasks. A task is running if         its start time is less than or equal to the current         processor clock and not all of its instructions have been         executed.</p>
</dd> <dt>Step 2.</dt> <dd>
<p>Determine the current priorities of the running tasks         and which of the running tasks are <em>blocked</em>. A         running task $T$ is         blocked if the next instruction in          $T$ is to lock         resource&nbsp;$k$ and         either resource&nbsp;         $k$ is already owned or at least         one other task owns a resource&nbsp;         $\ell $ whose priority ceiling is         greater than or equal to the current priority of         $T$. If          $T$ is blocked, it is said to be         blocked by every task owning such          $k$ or          $\ell $. The current priority of a         task $T$ is the         maximum of $T$¡¯s base         priority and the current priorities of all tasks that         $T$ blocks.</p>
</dd> <dt>Step 3.</dt> <dd>
<p>Execute the next instruction of the non-blocked running         task (if any) with the highest current priority. If there         was no such task or if a compute instruction was executed,         increment the processor clock by one&nbsp;microsecond. If a         lock or unlock instruction was executed, do not increment         the clock.</p>
</dd> </dl>
<p>The Priority Ceiling Protocol defined above has the     following properties:</p>
<ul class="itemize">
<li>
<p>Current priority is defined in terms of current priority         and blocking, and blocking is defined in terms of current         priority. While this may appear circular, there will always         be a unique set of current priorities that satisfy the         definitions.</p>
</li>
<li>
<p>All tasks will eventually complete.</p>
</li>
<li>
<p>There will never be a tie in step&nbsp;3.</p>
</li>
</ul>
<h3>Input</h3>
<p>Multiple test cases. Please process until EOF is reached. For each test case:</p>
<p>The first line of the input contains two integers     $t$      $(1 \leq t \leq 20)$, which is the     number of tasks, and $r$     ($1 \leq r \leq 20$),     which is the number of resources. This is followed by     $t$ lines, where the     $i^\text {th}$ of these     lines describes task $i$.     The description of a task begins with three integers: the     task¡¯s start time $s$     ($1 \leq s \leq 10\,     000$), its base priority      $b$ ($1     \leq b \leq t$), and an integer      $a$ ($1     \leq a \leq 100$). A task description is concluded by a     sequence of $a$ strings     describing the instructions. Each string is a letter     (<tt class="ttfamily">C</tt> or <tt class="ttfamily">L</tt> or     <tt class="ttfamily">U</tt>) followed by an integer. The string     <tt class="ttfamily">C</tt> $n$ ($1     \leq n \leq 100$) indicates a sequence of      $n$ compute instructions. The strings     <tt class="ttfamily">L</tt> $k$ and <tt class="ttfamily">U</tt>$k$     ($1 \leq k \leq r$)     indicate instructions locking and unlocking resource     $k$ respectively.</p>
<p>No two tasks have the same base priority.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>For each task, display the time it completes execution, in     the same order that the tasks are given in the input.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 1
50 2 5 C1 L1 C1 U1 C1
1 1 5 C1 L1 C100 U1 C1
70 3 1 C1
3 3
5 3 5 C1 L1 C1 U1 C1
3 2 9 C1 L2 C1 L3 C1 U3 C1 U2 C1
1 1 9 C1 L3 C3 L2 C1 U2 C1 U3 C1
<strong>Output:</strong>
106
107
71
8
15
16
</pre>