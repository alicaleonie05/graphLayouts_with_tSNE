# Graph Layouts using t-SNE

Generating Graph Layouts using openTSNE.<br>
<br>
Graphs are an ubiquitous form of data, used to describe for instance relationships in a
social network or citations between papers. To obtain a reasonably good embedding of a graph
in two dimensions, many graph layout methods have evolved. One big branch of those methods
are force-directed methods. In this work we present Graph t-SNE as a new force-directed dimensionality reduction method that enables graph embeddings of comparable quality to existing
methods. Therefore, we used an open source library for t-SNE for all our implementations
and show embeddings of several distinct benchmark datasets which can be obtained without the
need to develop a novel algorithm. We investigated the framework with different initializations, with altering the exaggeration value and varying the degree of freedom for the low-dimensional similarity t-kernel.<br>
<br>
In this project we generate graph layouts of two structural datasets in Layouts_StructuralGraphsGraph using generateLayouts.ipynb<br>

Can_96 and dwt_1005 are two structural datasets containing 96 nodes and 768 edges, and 1005 nodes and 8621 edges, respectively. Both are obtained from the SuiteSparse Matrix Collection (formerly: Florida Sparse Matrix Collection),
publicly available on https://sparse.tamu.edu/ (Davis and Hu 2011). For dwt_1005 c.f. https://math.nist.gov/MatrixMarket/data/Harwell-Boeing/dwt/dwt_1005.html. <br>

We use openTSNE (https://opentsne.readthedocs.io/en/stable/) and NetworkX (https://networkx.org/) to obtain the two-dimensional graph layouts/embeddings.<br>
We input the normalized and symmetrized adjacency matrix of the graph to the t-SNE optimization, which will use these affinities to obtain a two-dimensional embedding.<br>

<br>
<strong>Requirements</strong> <br>

python 3.10.0 environment with<br>
&nbsp; networkx 2.8.4 <br>
&nbsp; openTSNE 0.6.2 <br>
&nbsp; sklearn 1.1.3 <br>

<br>
<br>
This project comes from a laboratory rotation during my masters thesis in Neural Information Processing at the University of Tübingen.
In this folder you also find the report and the slides for a presentation. 
