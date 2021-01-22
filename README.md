# jan2021revision

# plc
[COMS20007 GitLab](https://cs-uob.github.io/COMS20007)

## 

### Turing Computablility

A language is said to be Turing-recognisable or recursively enumerable, just if it is recognised by some Turing machine.

A language is said to be co-Turing-recognisible or corecursively enumerable, just if its complement is recognised by some Turing machine.

A language is said to be Turing-decidable or recursive, just if it is decided by some Turing machine.

Theorem: A language is Turing-decidable iff it is both Turing-recognisible and Turing-corecognisible.

### Turing Reductions
Language A⊆Σ∗ is mapping reducible to language B⊆Σ∗, written A≤mB just if there is a computable function f:Σ∗→Σ∗ such that, for all w∈Σ∗:
w∈A iff  f(w)∈B

The function f is called the reduction.

Lemma: If A≤mB then Ac≤mBc.

Theorem: If A≤mB and B is Turing-recognisible then A is Turing-recognisible.

Corollary: If A≤mB and A is not Turing-recognisible, then B is not Turing-recognisible.

Corollary: If A≤mB and A is not co-Turing-recognisible, then B is not co-Turing-recognisible.

Corollary: If A≤mB and A is not Turing-decidable, then B is not Turing-decidable.

## Useful strategies:

- To prove L is turing recognisable, give the machine that recognises it. This must exist if L is TR by def
- To prove L is NOT Turing Decidable then reduce A_tm to it (or reduce any Non-TD L to it)
- To prove L is Turing decidable show both L and L^c are Turing recognisable
- Lots of questions require two way proofs - usually if there is an *iff*



# alg

### lemmas & statements

#### Trees

FLOT: Lemma: The following are equivalent for an n-vertex graph T = (V , E):
 - (A) T is connected and has no cycles, i.e. is a tree;
 - (B) T has n − 1 edges and is connected;
 - (C) T has n − 1 edges and has no cycles;
 - (D) T has a unique path between any pair of vertices.

DFS Tree:
- Key Fact: if x and y are adjacent, then x is an ancestor of y or vice versa.

BFS Tree: 
- Key Fact: If {x, y} is an edge in G, then x and y cannot be more than one layer apart in T, i.e. |d(v, x) − d(v, y)| ≤ 1.

#### Euler Walk
- a graph has a closed Euler walk if and only if it is connected and each of its vertices has even degree; hence every vertex of G has even degree. 

[Blackboard](https://www.ole.bris.ac.uk/webapps/blackboard/content/listContent.jsp?course_id=_240782_1&content_id=_4562987_1)


