---
layout: post
title: "VTDP: Find Local Network Patterns" 
--- 

It is common in working with network data to be much more interested in short path relationships between nodes than in nodes that are connected by longer paths. Cognitive tasks are to discover what is connected to a particular node, how the nodes are connected and what is the pattern of connections? Both node and link attributes may be important. 

**Example 1:** Who knows who in a social network? What are the relationships between them? 

**Example 2:** In a sofware diagram what modules depend on a particular node? What modules does it depend on?

###IMPLEMENTATIONS 

###Static Diagram 

A non-interactive diagram node link diagram is the most common solution with attributes of entities graphically encoded in the nodes and the attributes of relationships encoded using graphical properties of the links. 

**Guideline:** A fixed layout diagram is useful where the number of nodes is <30 and the node degree is < 3 for all nodes. 

###Degree of Relevance Highlighting 

In degree of relevance highlighting, [^1] and [^2], touching a node causes near neighbors and their links to become highlighted. A path radius of two or three is used for highlighting obtained through a breadth first search beginning with the selected node. The advantage of this method is that it enables substantially larger graphs to be rapidly explored. The method works with graphs 30 > n > 500. where n is the number of nodes. Also, there can be no high degree nodes. The problem with high degree nodes is that selecting one of them can cause too much of the graph to be highlighted yielding little useable information. 

<iframe src="http://assets.oculusinfo.com/demos/vtdp/local-network-patterns/index.html" width="750" height="725"></iframe>

###Visual thinking process with degree of relevance hightlighting  

*Display environment: A display containing many symbols representing entities linked by a complex overlapping set of relationships.*

1. *Construct visual query to find a symbol that may lead to useful information (information scent).
    Execute an epistemic action by selecting a symbol.*
2. *Computer carries out a breadth first search to a predetermined depth (e.g. 2) and highlights all nodes and edges within that range.* 
3. *Execute a visual query pattern among highlighted symbols to interpret highlighted information.*
4. *If a very high relevance pattern is found, execute an epistemic action to drill down for additional information. Usually this will be presented in a different display window.*
5. *Repeat from 1 as needed, cognitively marking visited symbols.*
 
**Use Guideline:** Consider using degree of relevance highlighting with medium sized network diagrams (30<n<500) where there are no high degree nodes. 

**Perceptual Guideline:** The highlighting method should be preattentive. This means that it should be distinct from color or shape codings already used in the diagram. Motion or blinking should be considered as a highlighting method that minimally interferes with the visual appearance of nodes and links. 

**Cognitive Guideline:** In a complex diagram it may be difficult to remember parts of the diagram that have already been explored. An ability to build up patterns and extract them is likely to be needed. 


###References 

[^1]: Munzner, T., Guimbreti6re, E, and Robertson, G. (1999). Constellation: A visualization tool for linguistic queries from MindNet. Proceedings of the 1999 IEEE Symposium on                Information Visualization, 132-135, San Francisco, CA, October 25-26, 1999. 
[^2]: Ware, C. Gilman, A.T. and Bobrow, R.J.  (2008). Visual Thinking with an Interactive Diagram. Lecture Notes in Artificial Intelligence.  5223. 118-126.  
 
 
 