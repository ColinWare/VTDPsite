---
layout: post
title: "Design Methodology"
---

VTDPs are intended as tools for the designer to use in reasoning about
visualization design.  The following paragraphs sketch out the design process as
a series of steps. In most cases these steps should be part of a spiral design
methodology, with multiple iterations.

### Step 1: High level cognitive task analysis

At the start of the design process the team members must establish, in a general
way, the problem to be solved by the final product. Initially, the description
should not specify the implementation method so as not to prejudge the solution.
Refinement will come later.

### Step 2: Data inventory

It is important to know early on in the process what data is available that
bears on the cognitive goals, what is readily accessible, and what is likely to
be accessible only with time delays.  Sometimes confidentiality can be a
stumbling block.  Both the structure of the data and the semantics will be
important in defining the visualization.  Data can be enormously varied in its
properties, but the following list contains some of the attributes that are
likely to appear in any inventory.

**Quantity:**  Very big data requires different approaches beyond what applies to medium or small data.

**Structure:**  E.g. hierarchical, map layers, network, multi-dimensional discreet.

**Time to access:**  Sometimes real-time or near real-time is critical.

**Ease of access:**  Some data is readily accessible, however, it is also common for data to require new infrastructure, have explicit costs, or have security issues.

**Interrelationships and interdependencies:**

**Quality and reliability:**

**Potential for derived data products processing infrastructure:**

The data inventory process will almost certainly start to blend into step 3,
task refinement, because data is only important as it relates to task
requirements.

### Step 3: Refinement of cognitive task requirements

As the data is understood, the set of tasks can be refined. Knowing the
specifics of particular data objects will suggest additional questions that may
be addressed.  As a generally strategy it is useful to work top down, breaking
down the overarching goal into analytic questions about who, what, where, when
and how.   It is also important to establish interdependencies between tasks,
such as the order in which they must be performed. At some point specific
computer based tools may be invoked but this should be delayed as long as
possible.   Only part of an analytic problem is likely to be amenable to
solutions that use visualization and it is important to divide the problem into
aspects that can use visual thinking and aspects that use other forms of
thinking or computation.  The following aspects of a problem suggest a
visualization solution.

There must be a way of transforming the problem so that solutions are
discoverable through a visual pattern search. The task should not be so
repetitive and standardized that an automatic computer pattern search is more
appropriate.

### Step 4: Identification of VTDPs and visualizations that can bear on the task

This step is the key creative stage in the design process. It is best led by an
experienced designer who knows both the types and nature of visualization and
understands the VTDPs that can be used to make them cognitively efficient. The
process starts with analytic questions about who, what, when, where and how and
matches these to appropriate VTDPs. (more)

### Step 5: Design decision rules

Since VTDPs incorporate rules regarding when they are most effective, it is
possible to construct a set of rules for visualization problems that provide
guidelines for when the different methods can be applied.  For example, we have
constructed the system of rules below regarding techniques that can be applied
to the visualization of graphs as node link diagrams.

*Small graph (<30 nodes) static representation*

*Medium graph (>30,<600) degree of relevance VTDP*

*Large Graph (>600 < 5m)  use dynamic queries VTDP attributes to reduce graph size to get to degree of relevance VTDP (<600).*

*Very large graph ( >5m) Query by example VTDP may be needed. Start with example, computer finds similar, user selects to refine query.*

### Step 6: Prototype development

In order to test the cognitive affordances of design alternatives, it is
necessary to have some form of prototype.  This can be design sketches of key
screens, or a rapidly developed working application demonstrating key design
ideas but lacking full functionality. The purpose is to provide a basis for
reasoning about cognitive efficiency when the visualization is applied to the
cognitive tasks identified in step 3.

### Step 7: Evaluation Through cognitive walkthrough

The cognitive walkthrough should focus on critical or frequent tasks to ensure
that the cognitive execution will be efficient using the VTDPs.  Small groups
should talk through the steps, attempting to identify bottlenecks, such as
unreasonable memory load, or instances where repetitive work can be offloaded to
the computer. It is likely that new cognitive tasks will emerge during the
process and the list of cognitive tasks can be refined; links between cognitive
tasks may be revealed.

VTDPs can be used in the evaluation process simply by considering if each in
turn is applicable to the set of cognitive tasks, and the data to be
visualized. More information on when different VTDPs are applicable can be found
[here.](/pages/EvalCriteria.html)

### Step 8: Alpha and beta products

The final stages of design should apply the common techniques of developing
alpha and beta product versions that can be tested and refined through use in
problem solving.
