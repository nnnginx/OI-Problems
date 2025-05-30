<p>According to Wikipedia, "The Traveling Salesman Problem (TSP) is a problem in combinatorial optimization studied in operations research and theoretical computer science. Given a list of cities and their pairwise distances, the task is to find a shortest possible tour that visits each city exactly once.  The problem was first formulated as a mathematical problem in 1930 and is one of the most intensively studied problems in optimization. It is used as a benchmark for many optimization methods. Even though the problem is computationally difficult, a large number of heuristics and exact methods are known, so that some instances with tens of thousands of cities can be solved."</p>
<p>Fortunately, you won't have to solve TSP. You're working for a very clever traveling salesman who has already figured out the path he is going to take. All he needs from you is a quick way to figure out how far he traveled after every segment of his tour.</p>
<h3>Input</h3>
<p>The salesman kept detailed records of his travels. You'll be getting a series of lines of the form "Some text (X, Y)." indicating that the salesman has been at the point X kilometers east and Y kilometers north of the origin of a Cartesian plane.</p>
<h3>Output</h3>
<p>For each segment of the trip, output the total distance traveled up to that point as a line in the format "The salesman has traveled a total of D kilometers." Show three digits after the decimal point when printing D. Note that the salesman only travels in straight lines (even after a couple of drinks).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
I started out at (0, 5).
Then I traveled to (3.7, 5).
After a couple of drinks I wobbled to (2.7, 4).
The next morning I woke up near (4, 3).
I finished my journey in (-.2, 8).

<strong>Output:</strong>
The salesman has traveled a total of 3.700 kilometers.
The salesman has traveled a total of 5.114 kilometers.
The salesman has traveled a total of 6.754 kilometers.
The salesman has traveled a total of 13.284 kilometers.
</pre>