---
layout: post
title: "VTDP: Dynamic Queries"
--- 

In some data set all entities have the same set of attributes.  The attributes define the data dimensions and each entity can be thought of as a point in a multidimensional space. A set of sliders is provided that can narrow the range on each of many attributes. Each slider adjustment is an epistemic action, narrowing the range of what is displayed. 

**Example 1:** A database of houses is shown on a map with a symbol for each house. The user adjusts sliders to select the price, number of bedrooms, bathrooms, square footage of living space and distance from the nearest school [^1].

**Example 2:** A scatterplot shows the set of stocks traded on the New York Stock Exchange. The axes represent market capitalization and annual increase/decrease in value. The user adjusts sliders to select price/earnings, monthly gain. Radio buttons are used to select industry sector.

The method has most often been used with scatter plots and to a lesser extent time series plots, but it can work with ranges displayed on maps, and with node link diagrams where restrictions can be placed on the nodes or links.

### Visual thinking process with dynamic queries
-----------------------------------------------------

*Display environment: A display with symbols representing entities drawn from a set of multidimensional discrete data, with a set of controls that restricts the range displayed on each of the data dimensions.*

1. *User constructs task relevant visual query that can be addressed by viewing a subset of multi-dimensional discrete data defined by a hyper-box.*
2. *Execute two visual queries on display: (a) Is the number of targets small enough to make drill down feasible? and  (b) Is a pattern found or high relevance symbol visible?*
3. *If as a result of 2b a high relevance symbol is found, execute an epistemic action to drill down for additional information. Usually the results will be presented in a different display window.*
4. *Otherwise, execute an epistemic action, dragging a slider which causes the computer to adjust a range on a data dimension and display the modified subset of the data.*
5. *Repeat from 2 until task is successfully completed or abandoned.*

###Dynamic Queries Illustrated with Using Aperture JS

**Implementation Guideline:** Ideally, the update following slider manipulation is very rapid (<100 msec).

**Data Guideline:** If we assume that each dynamic query slider can be used to reduce the range selected to 10% of the original, then the number of objects that be interactively queried is > 10 to the power d where d is the number of dimensions. So five sliders will allow for 100,000 objects to be interactively viewed. If the goal is to get to a small number of objects for drill down then the final on-screen display should contain fewer than 10 objects.  

**Visual Query Guideline:** If additional attributes can be encoded in the data glyphs this can facilitate visual search for the sought after information.

### References

[^1]: Ahlberg, C., & Shneiderman, B. (1994, April). Visual information seeking: tight coupling of dynamic query filters with starfield displays. In Proceedings of the SIGCHI conference on Human factors in computing systems (pp. 313-317). ACM.
 

 

 	 	 	 	 