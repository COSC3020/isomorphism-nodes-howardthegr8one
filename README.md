[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12782892&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

# My proof:

Using proof by contradiction assume that two graphs, $A$ and $B$ do not have the same 
number of nodes and are isomorphic. Since $A$ and $B$ are isomorphic then there exists
a one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$. However this mapping will create a contradiction. 

Since our graphs do not have the same number of nodes then either $A$ will have fewer
nodes than $B$ or vice versa. In the case where our function maps all nodes from $A$ to
$B$ and $A$ has fewer nodes than $B$ then every node from $A$ will be mapped to $B$ and 
there will still be nodes in $B$ that cannot be mapped to $A$ since every node in $A$
has been mapped. Since there are nodes that cannot be mapped then we do not actually
have a one-to-one function, therefore if $A$ and $B$ do not have the same number of 
nodes then they cannot be isomorphic.
