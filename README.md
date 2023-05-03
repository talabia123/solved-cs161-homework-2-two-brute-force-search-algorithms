Download Link: https://assignmentchef.com/product/solved-cs161-homework-2-two-brute-force-search-algorithms
<br>
The first two problems are to implement two brute-force search algorithms: depth-first and depth-first iterative-deepening. The search trees will be represented as lists in which a leaf node is represented by an atom, and a non-leaf node is represented by a list of its child nodes. For example, the list ((W X) (Y Z)) represents the complete two-level binary tree shown below on the left, and the list ((A (B)) C (D)) represents the tree shown below on the right.

The third problem is to implement a depth-first iterative-deepening solver for the missionary-cannibal problem discussed in class using a code skeleton.

<ol>

 <li>Write a single pure LISP function, called DFS, that performs a depth-first search of a tree. The function should take a single argument that is the list representation of the tree, and returns a single, top-level list of the terminal nodes in the order they would be visited by a right-to-left depth-first search.  For example, (dfs ‘((A (B)) C (D))) would return (D C B A). Do not use any auxiliary functions.</li>

 <li>Write a <em>set</em> of pure LISP functions that implement depth-first iterative-deepening. Your top-level function, called DFID, should take two arguments, the list representation of the tree, and an integer representing the maximum depth of the tree, and returns a single top-level list of the terminal nodes in the order that they would be visited by a right-to-left depth-first iterative-deepening search. Note that those nodes that are visited in multiple iterations will appear multiple times in the output list. For example, (dfid ‘((A (B)) C (D)) 3) would return (C D C A D C B A).</li>

</ol>

Each of these functions must work for trees of arbitrary depth and branching factor, and hence you may not assume any a priori upper bound on these parameters. Be sure to exhibit sufficient test cases to convince yourself and us that your programs work in general. Try at least the examples above, as well as the list (A (B C) (D) (E (F G))).

<ol start="3">

 <li>Implement a depth-first iterative-deepening solver for the missionary-cannibal problem that was described in class. To implement this solver, we provide you with a code skeleton (hw2_skeleton.lsp). Implement the functions in the code skeleton as described in their associated comments. DO NOT CHANGE THE FUNCTION NAMES OR PARAMETERS. Also do not write any additional functions.</li>

</ol>


