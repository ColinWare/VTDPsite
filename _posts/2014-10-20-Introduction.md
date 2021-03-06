---
layout: post
title: "Introduction"
---

We all think visually, some of the time. For the most part we are unaware that
we are visual thinking, as in the case that we thread our way through a crowded
room, or when we arrange groups of chopped vegetables and other ingredients on a
countertop in preparing to cook a complicated dish.  Graphic designers may think
consciously of design decisions, analyzing which combination of colors and forms
most clearly conveys the required information, but they are in the minority.

We also use visualizations as thinking tools. Many people who work creatively,
construct rough and ready sketches, which are often unintelligible to anyone
else, that somehow help them organize their thoughts. Those abstract squiggles
hint at different ways of partitioning physical space or the space of ideas or
even both together.

Visualizations are tools for reasoning about data and to be effective they must
support the activities of visual thinking.  Part of this is ensuring that data
is mapped to the display in such a way that informative patterns are available
to resolve visual queries concerning the cognitive task. This requires matching
the graphic representation with the capabilities of human visualization.  For
example, correlations between variables should be visually easy to see and
commonly searched for symbols should be more distinctive than those that are
rarely sought out.  In addition, interactions must be designed to support an
efficient visual thinking process. Visual analytics is an example of distributed
cognition and cognitively efficient interactions require that perceptual and
cognitive processes in the brain of the analyst must be efficiently linked to
computational processes in a computer. For example, data points representing
companies can be shown simultaneously in a map view and in a scatter plot view;
the technique of brushing can be applied so that points on the map, when
selected, are highlighted in both views. This can support reasoning about the
growth of industries related to geographic regions, but to be cognitively
efficient the brushing effect should ideally appear in less than a tenth of a
second.

Visual Thinking Design Patterns (VTDPs) are based partly on a prior construct
developed by Ware[^1] and called visual thinking algorithms (VTAs).  VTDPs
represent a broadening of this original concept with a change in emphasis. VTDPs
are a method for describing the combined human-machine cognitive processes that
are executed when interactive data visualizations are used as cognitive tools.

VTDPs take their inspiration from Alexander's design patterns[^2] intended for
architects and from design patterns developed for software engineering[^3].
Although considerable research has shown that perceptual and cognitive
principles can be applied usefully to the design of interactive visualization,
this knowledge is only applied in practice if a particular designer has taken an
interest in the relevant research.  VTDPs are intended to provide an accessible
structured method for combining knowledge about interaction methods and
visualization designs together with cognitive and perceptual principles.

Like their precedents, VTDPs are intended to describe best practice example
solutions to design problems where interactive visualization is an intended
component. VTDPs provide a method for taking into account perceptual and
cognitive issues especially key bottlenecks in the visual thinking process, such
as limited visual working memory capacity.  They also provide a way of reasoning
about semiotic issues in perceptual terms via the concept of the visual query.
VTDPs incorporate the common set of interactive techniques used in visualization
and suggest how they may be used separately or in combination. VTDPs should be
understandable with a modest amount of training, and it should be possible to
incorporate them into common design practices. VTDPs are potentially applicable
to all visualization design problems, including design of presentation
materials, interactive training materials and analytic tools.  The following
section concentrates on a single application domain, the design of visualization
tools used in visual analytics.

Like software engineering and architectural design patterns, VTDPs are not
modules and are not reusable.  The demands of analysis are almost infinitely
varied due to the enormous variety of data types and analytic problems.  As a
result, any modularization of VTDPs would necessarily restrict the domain.
Nevertheless, implementations of VTDPs can take advantage of modular components.
For example, map display software may allow for extra magnifying windows which
can be used to support the pattern comparisons in a large information VTDP
space.

------

### References

[^1]: C. Ware, Information Visualization, Perception for Design, Third Edition.  Morgan Kaufman. 2012.
[^2]: C. Alexander, S. Ishikawa, and M. Silverstein, A pattern language. Oxford University Press. 1977.
[^3]: E. Gamma, R. Helm, R. Johnson, and J. Vlissides. Design Patterns: Elements of Reusable Object-Oriented Software. Addison-Wesley. 1995.
