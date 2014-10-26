---
layout: post
title: "VTDP: Cognitive Reconstruction"
---

Most analysts will have their workflow frequently interrupted. They also often need to extend or redo prior analytic work as new data becomes available. Successfully resuming a prior analysis requires that the entire cognitive system be reconstructed and this involves rebuilding both the machine state and the operator state. It is a mistake to think of the human side of this as an operation where information is simply loaded from long term memory. All long term memory is more a process of reconstruction than a process of retrieval.

**Example:** An analyst works on a project for a few hours. Because of a major crisis she is asked to switch tasks for three days. She then returns to first project. 

### The cognitive reconstruction process  

1. An analyst works uses the system to make notes describing:
  1.1 discoveries, significant data objects, reasoning behind data manipulations.
1. The system stores a record of all data transformations. 
2. User requests that the computer system save the state of analytic work in progress and closes the system. 
3. At a later date, the user requests that the system re-load the state to continue the analysis from that point.  
4. User attempts to reconstruct the key elements of the user's own cognitive landscape from long term memory with the following questions in mind: 
  - What were the short and medium term goals associated with that prior state?  Notes will be read, emails reviewed, stated goals reviewed.
  - What contextual information does the user remember relating to those goals; for example, people involved, organizational issues?.
  - What was the set of software tools used and the sequence of operations to achieve the system state. 
5. Cognitive work progresses. 


There are important tradoffs in how the cogntive reconstruction task should be supported in a software system. In much exploratory data analysis, frequent note taking would get in the way of thinking about the problem, and much of the activity is sifting through irrelevant material that is not worth saving.

**Use guideline:** Effort in note taking < Later savings in cognitive reconstruction. 
It is also the case that saving a detailed interaction history has no value if it will never be re-visited, or where the cost of retracing an analysis is greater than the cost of redoing the analysis.

**Implementation guideline:** Effort in storing analytic operations < Later savings in cognitive reconstruction. 

Finally, there is the case of specialized analytic tools where full support for note taking and storing sequences of analytic operations may require a very considerable development effort, it may involve data bases and archiving facilities. This may be worth less in aggregate than having the analyst take notes on paper for the few times the tool is used. 