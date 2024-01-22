# clusters

https://www.jmlr.org/papers/volume9/vandermaaten08a/vandermaaten08a.pdf?fbcl

https://dl.acm.org/doi/pdf/10.1145/233269.233324

Birch Highlights
- Makes clusters based on data thats close to each other instead of analyzing all data.
- It treats dense data more importantly than outliers.


Clustering is done using a CF Tree algorithm.  The tree is used in Birch to very quickly cluster a large dataset.  When this tree is constructed, we can use each subcluster as a single point, then use an existing algorithm for modification.

Phase 1: Constructs the tree
Phase 2: Possibly runs other algorithms on the tree
Phase 3: Runs k-means with n number of clusters on this tree.

