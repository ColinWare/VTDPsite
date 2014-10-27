---
format: post
title: "VTDP: Pattern Comparisons in a Large Information Space" 
---

Sometimes we need to compare details in a large information space such as a high resolution image or a large and complex network. Cognitive tasks are to find similarities and differences between small scale patterns.  

**Example 1:** A map display where we need to compare small scale geological features on one part of a map with small scale features in another part of a map.  

**Example 2:** An X-ray image where we need to compare widely separated small stuctures possibly representing cancerous nodules. 

**Example 3:** A net work diagram showing metabolic pathways in a cell. We need to compare small sub systems of metabolic pathways across species. 

Any pattern comparison involves loading some aspect of one pattern into visual working memory, to be later compared to some other pattern.  Pattern comparisons are far more efficient if the transfer of attention between one pattern and another can be made using eye movements, because in this case the information only needs to be held for a fraction of a second. 

### An overview of the process of visual pattern comparisons  
```
1. *Execute an epistemic action by navigating to location of first pattern.*
2. *Retain subset of first pattern in visual working memory.*
3. *Execute an epistemic action by navigating to candidate location of a comparison pattern.*
4. *Compare working memory pattern with part of pattern at candidate location.*
    4.1  *If a suitable match is found terminate search.*
    4.2  *If a partial match is found,  navigate back and forth between candidate location and master.  pattern location loading additional subsets of candidate pattern into visual working memory and making comparison until a suitable match or a mismatch is found.*
5. *If a mismatch is found repeat* 
```

###IMPLEMENTATIONS

#### Zooming 

The simplest and most common implementation of the Pattern Comparisons VTDP is to allow for zooming (scale change) of the data display [^1].  However, since it can take several seconds to transition from one area of detail to another using this method it can be cognitively inefficient and place a burden on working memory.  

**Use Guideline:** Zooming is useful when comparisons are infrequent and where the patterns to be compared are simple. Consider using Magnifying Windows or Linked Snapshots when the patterns to be compared are more complex. 

**Implementation Guideline:** The optimal zoom rate is around a scale change of 4x/sec. 

#### Magnifying Windows 

Interactive magnifying windows can be attached by the user to focal points on an overview display. The focus of the window can be controlled either by dragging at the focal point. Additionally fine scale movement can be carried out by dragging in the magnifying window itself [^5]. The problem with this solution can be the overhead involved in setting up the extra windows.  If they are frequently needed they should always be present.  There are many tradeoffs in the amount of screen space devoted to magnifying windows and overview and the best design will depend on the specific application.



**Use Guideline:** Provide magifying windows when frequent comparisons of detailed areas are needed. These are especially valuable when the patterns to be compared exceed visual working memory capacity.

**Use Guideline:** The magnifying factor supported by a magnifying window should be less than 30x. 

**Cognitive Guideline:** Use extra windows when patterns to be compared are too complex to be held in visual working memory.
 
#### Snapshot Gallery with Zooming 

Small snapshots saved to a gallery supports side-by-side comparisons of complex patterns using eye movements. This method can be used to enhance zooming alone, or a viewer with magnifying windows. Links back to locations in the larger image can provide context. 



**Use Guideline:** Provide snapshot gallery support when frequent comparisons of many detailed areas are needed. 

**Implementation Guideline:** Provide links back to the originating image to give context. 

###Geometric Fisheye View 

In the geometric fisheye view, a data map is distorted so that some regions are magnified and others are minified to compensate [^2].  Distortion occurs at the boundaries between the different scales. Because of the distortion problem, large magnification factors should be avoided. Geometric Fisheye View can have multiple foci of magnification and this is useful for 

**Use Guideline:** Use geometric fisheye view support where comparisons can be made with < 5x magnification. 

###Nested Graph With Intelligent Zoom 

See also [VTDP: Drill Down, Close out with Heirarchical Aggregation] 

If the data for comparison is a large graph, or a set of large graphs, a form of fisheye view can be developed based on the nested structure of the graph. Several different subgraphs can be expanded and thereby compared. In the intelligent zoom method [^4] regions not expanded are contracted to save space. There are limitations on the complexity of the sub graphs that will inevitably limit comparisons. At the time of writing these limitations have not been quantified. 


**Guidelines:** To be determined 

###References

[^1]: Bederson, B. and Hollan, J. (1994). Pad++: A zooming graphical interface for exploring alternate interface physics. Proceedings of UIST "94, ACM, 17-36. 
[^2]: Carpendale, M. S. T., Cowperthwaite, D. J., & Fracchia, F. D. (1997). Making distortions comprehensible. In Proc IEEE Visual Languages, 36-45.
[^3]: Plumlee, M. and Ware, C. (2002). Modeling performance for zooming vs multi-window interfaces based on visual working memory. Advanced Visual Interfaces, Trento, Italy, May Proceedings, 59-68. 
[^4]: Schaffer, D, Zuo, Z, Bartram, L., Dill, D Dubs, S., Greenberg, S. and Roseman, M. (1993). Comparing fisheye and full-zoom techniques .for navigation of hierarchically clustered networks, in Proc. Graphics Interface (GI 93), 87-96.
[^5]: Ware, C. and Lewis, M. (1995). The DragMag image magnifier. CHI '95 Conference Companion and Conference Video Proceedings, ACM, 407-408. 
 
    
  
