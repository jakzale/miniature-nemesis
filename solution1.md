Problem 1 - Solution
================

**Note** Because I am extremely busy at the moment this solution will not be explained thoroughly. I will add more detailed explanation later.

Problem Analysis
------------------------

The problem can de expressed in certain mathematical terms as an undirected graph, where *ports* are the nodes and *sea routes* are the edges.

In order to verify a tale it is necessary to find out if it is possible to traverse from the starting node ```A``` to destination node ```B``` given ```n``` amounts of steps.
Because it is possible to travel between nodes in both ways and visit certain nodes more than once, an existing path of ```m - 2``` edges between ```A``` and ```B``` will verify a tale of from ```A``` to ```B``` using ```m``` steps.  
Since the relation is recursive, it is possible to express it using parameter ```k```: ```m - 2k, k >= 0``` , and given the properties of natural numbers it is possible to express it in a following way:  
> Tale from ```A``` to ```B``` with ```n``` steps is valid if there exist a path of length ```m, m <= n``` between ```A``` and ```B``` and both ```n``` and ```m``` are either **odd** or **even**.

**EDGE CASE 1**
When ```A = B```, a tale with even steps is valid if there exist a node ```C``` adjacent to ```A```.

**EDGE CASE 2**
When ```A = B```, a tale with odd steps of length ```k``` is valid if there exist a node ```C``` and there exist two paths from ```A``` to ```C``` of length ```m``` and ```n``` respectively, given that ```m``` is odd and ```n``` is even and ```m + n <= k```.

Algorithmic Implementation
-------------------------------------
Will add that in a second.

