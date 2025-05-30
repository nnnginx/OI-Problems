<style>
	.center {
		margin-right: auto;
		margin-left: auto;
	}

	.example-table {
		margin-top: 10px;
		text-align: left;
		width: 100%;
	}

	.example-table td {
		max-width: 0;
		word-wrap: break-word;
		vertical-align: top; 
	}

	.example-table .vertical-spacer {
		height: 5px;
	}

	.section {
		margin-top: 19px;
		margin-bottom:19px;
	}

	.section:first-child, .section:first-child > h3:first-child {
		margin-top: 0;
	}

	.paragraph {
		margin-top: 10px;
		margin-bottom: 10px;
		text-align: left;
	}

	.paragraph ul, .paragraph pre {
		margin-top: 3px;
		margin-bottom: 3px;
	}

	pre {
		tab-size: 4;
	}

	.billboard {
		line-height: 1em;
		outline: solid 1px black;
	}
</style>

<div>
	<div class="section">
		<h3>Description</h3>
		<div class="paragraph">
			A <em>tree</em> is a connected acyclic graph.
		</div>
		<div class="paragraph">
			A <em>binary tree</em> is a tree for which each node has a left child, a right child, both, or neither, e.g.
		</div>
	<pre class="center" style="width:9ch">    1
   / \
  2   3
 / \   \
4   5   6</pre>
		<div class="paragraph">
			There are three common ways to recursively traverse such a tree.
			<ol>
				<li>Preorder: parent, left subtree, right subtree</li>
				<li>Postorder: left subtree, right subtree, parent</li>
				<li>Inorder: left subtree, parent, right subtree</li>
			</ol>
		</div>
		<div class="paragraph">
			Given preorder, postorder, and inorder traversals, determine if they can be of the same binary tree.
		</div>
		<div class="paragraph">
			For example,
	<pre class="center" style="width:11ch">1 2 4 5 3 6
4 5 2 6 3 1
4 2 5 1 3 6</pre>
			are the preorder, postorder, and inorder traversals of the tree above.
		</div>
		<div class="paragraph">
			But
<pre class="center" style="width:11ch">1 2 4 5 3 6
4 5 2 6 1 3
4 2 5 1 6 3</pre>
			cannot be the preorder, postorder, and inorder tranversals of the same binary tree.
		</div>
	</div>

	<div class="section">
		<h3>Input</h3>
		<div class="paragraph">
			The first line is the number of nodes in each traversal, 0 &lt; N &lt;= 8000.
			<br>
			The second line is the N space seperated nodes of the preorder traveral.
			<br>
			The third line is the N space separated nodes of the postorder traversal.
			<br>
			The fourth line is the N space separated nodes of the inorder traversal.
		</div>
		<div class="paragraph">
			Each traversal is a sequence of the nodes, numbered 1 to N, without repitition. 
		</div>
	</div>

	<div class="section">
		<h3>Output</h3>
		<div class="paragraph">
			Print "yes" if all three traversals can be of the same tree, and "no" otherwise.
		</div>
	</div>

	<table class="section example-table">
		<tbody><tr>
			<th>Input</th>
			<th>Input</th>
		</tr>
		<tr>
			<td>
<pre>6
1 2 4 5 3 6
4 5 2 6 3 1
4 2 5 1 3 6</pre>
			</td>
			<td>
<pre>6
1 2 4 5 3 6
4 5 2 6 1 3
4 2 5 1 6 3</pre>
			</td>
		</tr>
		<tr>
			<th>Output</th>
			<th>Output</th>
		</tr>
		<tr>
			<td>
<pre>yes</pre>
			</td>
			<td>
<pre>no</pre>
			</td>
		</tr>
	</tbody></table>
</div>