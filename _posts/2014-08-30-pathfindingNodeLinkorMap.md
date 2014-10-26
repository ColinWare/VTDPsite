---
layout: post
title: "VTDP: Pathfinding Using a Node-Link Diagram or a Map"
---

In a typical node-link diagram entities are given by the nodes and relationships are given by the links between them. Relationships between entities are discovered by finding the paths between them. 

**Example:** Given a social network diagram showing communication channels between individuals, discover the possible pathways whereby information may have travelled from one individual to another. This example is also used in the VTDP Visual Query. 

**Example:** Find a route on a road map between one location, denoted by a symbol, and another. 

 
###The path finding process 

Display Environment: A node-link diagram with symbols representing nodes and colored lines representing links between nodes. Alternatively, a roadmap with symbols representing cities, and colored lines representing roads between the cities. 

1. Conduct a visual search to find node symbols representing start and end points.
2. Mark these in mental map of display space.
3. Fixate the start symbol.
  3. 1 Extract patterns corresponding to connecting lines of a particular color that trend in the right          overall  direction.  
  3. 2 Mentally mark the end point symbol of the best candidate line.
4. Repeat from 3 using new start point until end point is located.
5. Push information concerning the path to logical propositional store (only a cognitive hint is needed       because the path can be easily reconstructed.)
6. Repeat from 3 to find alternative candidate paths, avoiding paths already found.


Graph drawing is an academic field in which the major goal is to lay out graphs so that the links between nodes are clear. Some of the important principles are:

- Minimize link crossings, especially avoid edge crossings at acute angles.
- Keep path lengths short, especially for important paths.
- Avoid having links cross nodes where there is no connection to the node. 

For simple networks < 30 nodes and < 45 links, a clear 2D non interactive layout many be possible. When there are more nodes than this interactive methods can be used.

For more related information see 
[VTDP: Drill Down-Close Out with Hierarchical Aggregation](http://www.visualthinkingdesign.com/drillDownHeirarchy/), and [VTDP: Find Local Network Patterns.](http://www.visualthinkingdesign.com/localNetworkPatterns/) 

When the links in a network are weighted and the networks are complex, algoritms may be useful in finding the shortest paths. An example is finding routes with a road map; in this case there are weights for the distance between junctions and weights for the speed or travel along road segments. 

  
 
    
  