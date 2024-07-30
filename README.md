# Graph Layouts using t-SNE

Generating Graph Layouts using openTSNE.<br>
<br>
Generate graph layouts of can_96 and dwt_1005 in Layouts_StructuralGraphsGraph using generateLayouts.ipynb<br>

can_96 and dwt_1005 - Two structural datasets containing 96 nodes and 768 edges, and 1005 nodes and 8621 edges, respectively. Both are obtained from the SuiteSparse Matrix Collection (formerly: Florida Sparse Matrix Collection),
publicly available on https://sparse.tamu.edu/ (Davis and Hu 2011). For dwt_1005 c.f. https://math.nist.gov/MatrixMarket/data/Harwell-Boeing/dwt/dwt_1005.html. <br>

We use openTSNE (https://opentsne.readthedocs.io/en/stable/) and NetworkX (https://networkx.org/) to obtain the two-dimensional graph layouts/embeddings.<br>
We input the normalized and symmetrized adjacency matrix of the graph, to the t-SNE optimization, which will use these affinities for optimization of a two-dimensional embedding.<br>

<br>
<strong>Requirements</strong> <br>

python 3.10.0 environment with<br>
&nbsp; networkx 2.8.4 <br>
&nbsp; openTSNE 0.6.2 <br>
&nbsp; sklearn 1.1.3 <br>
