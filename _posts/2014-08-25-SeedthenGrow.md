---
format: post
title: "VTDP: Seed then Grow" 
---

Often a data analyst starts with a particular seed of information and then begins to gather related information. Each additional information nugget may lead to further expansion of an information tree or network. This has been called "Start with what you know, then grow" [^1]. 

**Example 1:** Law is often based on precedents and legal researchers must follow chains of citations to discover rulings on similar cases. These data bases can be large. The researcher may start with a particular case and trace out a citation chain either forward or backwards to find related cases. 

**Example 2:** In law enforcement, criminal organizations can be discovered by starting with an individual and then determining their associates. The associates of those associates may also be examined, and so on. 

###An overview of the process of seed then grow 

Display environment: Data entities are represented as nodes. Links between them are represented as lines. 

1. *A node is added to the display space representing an entity.* 
2. *A mouse click epistemic action causes the system to search for related facts. These are displayed on the screen with lines linking them to the original node.* 
3. *The analyst visually searches the added nodes for information scene based on the information scent. If visual information scent is inadequate, apply VTDP drill down before proceeding.* 
4. *Nodes that appear unrelated are deleted (or hidden).* 
5. *For nodes that appear to be task relevant repeat from 2.*  

 
###Implementation: A left to right tree

The most basic implementation is a simple click and expand, with a box to support node closure. The path to the root reveals the lineage of a particular piece of information. 

![Tree structured data, expanded on demand](/images/tree2.jpg)
http://hcil2.cs.umd.edu/trs/2005-23/2005-23.html

**Data Guideline:** In its simple form this method will work best with problem sets where node degree < 30. In other words, expanding a node should result in fewer than 30 choices. 

**Problem Guideline:** Avoid long left to right chains which will move off screen and require scrolling, leading to cognitive inefficiencies where it is critical to perceive the path to the root. 

**Visual Scent Guideline:** Maximize the visual coding of variables if users will work extensively with the system and can be expected to learn the symbol system, or where already learned visual symbols exist. Otherwise coding using words will often be the best option. 

###The High Degree Node Problem 

The most common problem with the seed then grow approach is that of too many links. In graph theoretic terms these are called high degree nodes.  In many networks there may be thousands of connections for a single node. For example, the clients of a bank. It is not useful to click on a bank node and for customers to appear. The problem of deleting irrelevant nodes will hugely reduce the efficiency of the process. 

###Implementation: Tree with Fisheye View to Support Larger Trees 

Although the example below, from [^2], is not a see then grow application, it nicely illustrates how a fisheye view can be applied to make large horizontally laid out trees accessable. 
 
![Tree with fisheye](/images/MunznerTreeJuxtaposer.png)

###Implementation: Network with Degree of Relevance 

The VTDP seed then grow can also be used with a nework, rather than a tree. The example below used the VTDP Degree of Relevance method. The computer expands using nodes that are computed to be most relevant to the node selected [^3]. 

![Expandable graph](/images/vanHamPerer.png)

###References 
[^1]: Heer, J., and Boyd, D. (2005) Vizster: Visualizating online social networks. Proc. IEEE Information     Visualization. 32-39. 
[^2]: Munzner, T., Guimbretihre, F., Tasiran, S., Zhang, L., and Zhou. Y. TreeJuxtaposer: Scalable Tree      Comparison using Focus+Context with Guaranteed Visibility. SIGGRAPH 2003, 453-462. 
[^3]: Van Ham, F., & Perer, A. (2009). Search, Show Context, Expand on Demand: Supporting Large Graph         Exploration with Degree-of-Interest. Visualization and Computer Graphics, IEEE Transactions on, 15(6), 953-960.
 
 
 
 
    
  
