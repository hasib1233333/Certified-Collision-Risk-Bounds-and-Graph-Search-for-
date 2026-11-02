Title:

Certified Collision Risk Bounds and Graph Search for Path Planning on Spatially Correlated Occupancy Maps

Abstract:

Most risk-aware path planners for probabilistic occupancy maps compute the collision probability of a path as if the grid cells were independent. Maps built with Gaussian processes or Gaussian Markov random fields (GMRFs), however, are spatially correlated, and the exact path risk does not fit into graph search. We show that this correlation can be handled safely. If the latent covariance has no negative entries, correlation inequalities imply that the independence product remains a valid but conservative bound, and that pairing neighboring cells tightens it. If the latent precision matrix is an M-matrix, as in common GMRF priors and their posteriors after per-cell measurements, the Markov chain product is also a valid bound. These bounds add up along the path, so Dijkstra’s algorithm on a two-layer lifted graph optimizes them exactly, and Lagrangian relaxation decides feasibility for the chosen bound exactly while reporting an optimality gap. In 17,640 plans on 840 synthetic maps, a GMRF mapping pipeline and a public laser map, the certified planners kept the risk budget under the assumed map model, while threshold planners exceeded it on more than 90% of paths. At the strongest correlation, certified feasibility on cluttered maps rose from 53.3% to 91.7%.

Keywords:

Path planning; chance constraints; occupancy grid maps; Gaussian Markov random fields; correlation inequalities; total positivity; constrained shortest path
