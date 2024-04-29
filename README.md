[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/QM7QGF1q)
# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

-Based on work from last semester

We can prove that not all graphs that are isomorphic are compeletly connected by finding 
an example of two isomorphic graphs that arent completely connected.

Take the folowing graphs: A and B.

Graph A: 

    {'a': {'b': 7, 'c': 4},

    'b': {'c': 3, 'd': 8},

    'c': {'d': 5},

    'd': {'b':2}}

$V_1$ = (a,b,c,d)

Edges of A: $E_1$ = (a,b) (a,c) (b,c) (b,d) (c,d) (d,b)

Graph B: 

    {'w': {'x': 7, 'y': 4},

    'x': {'y': 3, 'z': 8},

    'y': {'z': 5},

    'z': {'x':2}}

$V_2$ = (w,x,y,z)

Edges of B: $E_2$ = (w,x) (w,y) (x,y) (x,z) (y,z) (z,x)


The graphs A and B not completeley connected since there is not an edge for every pair of vertices, but they are isomorphic according to the aformentioned
ormal definition of isomorphisim in that.

 $f: V_1 \rightarrow V_2$ such that $(u,v) \in E_1$ if $(f(u),f(v)) \in E_2$

We can see that all the nodes $V_1$ have an equivalent in $V_2$:

 f(a) -> w

 f(b) -> x

 f(c) -> y

 f(d) -> z

We can see that all the edges in the set $E_1$ have an equivalent in the set $E_2$

(a,b) -> (w,x) 
(a,c) -> (w,y) 
(b,c) -> (x,y) 
(b,d) -> (x,z) 
(c,d) -> (y,z) 
(d,b) -> (z,x)

 So we can conclude that not all graphs that are isomorphic are completely connected.

 






