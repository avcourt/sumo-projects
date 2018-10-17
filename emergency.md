Although SUMO-gui allows for visualization of emergency vehicles by setting the vtype attribute in our routes file. ('emergency', 'police', 'firebrigade', for ambulances, police and firetrucks). However, like the visualization of railway edges, this is really just a visual aid, and does not affect behaviour automatically. 

Induction loop variables => http://sumo.dlr.de/wiki/Simulation/Output/Induction_Loops_Detectors_(E1)
Script for generating E1 detectors (induction loops) for each junction in the supplied network file.
Execute the generateTLSE1Detectors.pyscript with --help option to get details about usage and available options. 

traffic light progrm definition

-sublane model



## Routing Algorithms

    dijkstra: (default) Dijkstras algorithm is the simplest and slowest of routing algorithms. It is well suited to routing in time-dependent networks (i.e. when the travel time on an edge depends on the time of day)
    **A**r: The A* routing algorithm uses a metric for bounding travel time to direct the search and is often faster than dijkstra. Here, the metric euclidean distance / maximumVehicleSpeed) is used.
        by using astar together with the option --astar.landmark-distance <FILE> the ALT-Algorithm is activated (A*, Landmarks, triangle inequality). It uses a precomputed distance table to selected network edges (so-called landmarks) to speed up the search, often by a significant factor.
        by using astar together with the option --astar.all-distances <FILE> the A* algorithm is used together with a complete (and often huge) distance table to allow for blazing fast search.





