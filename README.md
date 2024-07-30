# Graph Layouts using t-SNE

Generating Graph Layouts using openTSNE.<br>
<br>
Generate graph layouts of can_96 and dwt_1005 in Layouts_StructuralGraphsGraph using generateLayouts.ipynb<br>

can_96 and dwt_1005 - Two structural datasets containing 96 nodes and 768 edges, and 1005 nodes and 8621 edges, respectively. Both are obtained from the SuiteSparse Matrix Collection (formerly: Florida Sparse Matrix Collection),
publicly available on https://sparse.tamu.edu/ (Davis and Hu 2011). For dwt_1005 c.f. https://math.nist.gov/MatrixMarket/data/Harwell-Boeing/dwt/dwt_1005.html. <br>

We use openTSNE (https://opentsne.readthedocs.io/en/stable/) and NetworkX (https://networkx.org/) to obtain the two-dimensional graph layouts/embeddings.<br>
The input to the t-SNE embedding is a normalized and symmetrized adjacency matrix of the graph, treated as affinities, which will be used for optimization with t-SNE in a two-dimensional embedding.<br>

<br>
python 3.10.0 environment with<br>
&nbsp; networkx 2.8.4 <br>
&nbsp; openTSNE 0.6.2 <br>
&nbsp; sklearn 1.1.3 <br>
