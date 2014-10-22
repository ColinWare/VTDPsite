---
layout: post
title: "Components"
---

A VTDP is made up of a number of components including epistemic actions - these
are actions to obtain further knowledge, perceptual requirements, memory loads,
and a description of the visual thinking process that occurs during problem
solving.

A VTDP begins with a statement of the problem it is designed to solve, together
with one or more examples. In most cases it will contain a pseudo-code
description of the combined cognitive process and this will typically
incorporate many the following components.

### Perceptual and Cognitive Operations

These include converting some part of a problem into a visual query, mentally
adding both imagery and attributes to a perceived symbol or other feature.
Cognitive operations include decisions such as terminating a visual search when
an item is found.  A key bottleneck in cognitive processing is the capacity of
visual working memory, so situations where visual working memory limits can lead
to cognitive inefficiently are elucidated, and solutions described.

### Visual Queries

An aspect of a problem is cognitively transformed so that progress can be made
using a visual pattern search. For example, finding a relationship in a social
network diagram will involve visually tracing a line linking two nodes.  Visual
queries provide a method for reasoning about key problems of data
representation.

### Visual Pattern Processing

A visual pattern is the target of a visual query. The goal of efficient graphic
design is to ensure that data is mapped into graphical form in such a way that
all probable visual queries can be efficiently executed.  Most complex design
problems involve tradeoffs; therefore, the pattern mappings for more frequent or
more important visual queries should be more salient.

### Working Memory Load

Working memory capacity is assumed to be at most 4 simple patterns or shapes if
the patterns are previously unknown. If patterns are well known, a skilled
analyst can remember many more as well as more complex patterns.

### Epistemic Actions

These are actions designed to seek information. They include mouse movements to
select data objects, causing them to reveal more about their attributes, and
panning and zooming actions to navigate through a data space. This is a
broadening of Kirsh and Magio's[^1] initial concept. It goes beyond
manipulations of the environment to include actions that do not actually change
the environment but are nevertheless executed to gain knowledge. These include
eye or head movements to pick up detailed information from different parts of a
display.[^2]

### Externalizing

These are instances where someone saves some knowledge gained, by putting it out
into the world, for example, by adding annotations to a visualization, or
checking boxes to indicate that certain information is deemed important or
irrelevant.

### Interaction Driven Computation

This includes all parts of a visual thinking algorithm that are executed in a
computer. Of particular relevance to VTDPs are computations that rapidly change
how information is displayed. This can be as simple as zooming or changing the
range of the data that is displayed because of user interaction.

### Display Budget

The display budget is the amount of visual information that can be usefully
displayed at a given time.  For example, there is no point in displaying a graph
with 5000 nodes if very few of them can be visually resolved.

### The VTDP Virtual Machine

When thinking about interactive systems, it is useful to consider the simple
virtual machine, illustrated below.  This contains a simple visualization
pipeline as well as the key components of perceptual and cognitive processing.
Very often, a gain in cognitive efficiency can be achieved by shifting part of
the workload from visual working memory by means of simple computations and
interactive methods. The basic elements of the visual thinking virtual machine
are shown below.

![Visual Thinking Virtual Machine](/images/VTDPsVirtualMachine_w.png)

------

### References

[^1]: Kirsh, D., and Maglio, P. (1994) On Distinguishing Epistemic from Pragmatic Action. Cognitive Science, 18, 513-549.
[^2]: Ware, C. (2012) Information Visualization: Perception for Design. 3rd Edition. Morgan Kaufman.
