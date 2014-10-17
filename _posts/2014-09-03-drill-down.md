---
layout: post
title: "VTDP: Drill Down"
---

 In data visualization “drilling down” is the name given to the epistemic
action whereby more information is obtained about a symbolically displayed
entity (Shneiderman called this "details on demand"[^1]).

**Example:** a real estate map with symbols representing houses for sale. The
user clicks on a symbol to get details of the listing. Drill down is useful in
almost all visualizations. In cases where there are many symbols on a screen
it is important that symbols represent as much information scent as possible
otherwise the analyst may have to drill down and view a great deal of
irrelevant information. Scent consists of a set of graphical attributes or
words that represent a summary of the information referenced by the symbol.

### The Drill Down Process

*Display Environment:* Symbols representing data entities, some kind of
selection device.

1. Conduct a visual search, based on information scent, for most task relevant symbol.
2. Select symbol.
3. Computer displays detailed information. Repeat from 1 as task demands.

The marking of previously visited symbols can be done either mentally or by
using a cognitive externalization, such as checking off symbols that failed to
yield useful information.

### Fundamental Limits on Drill Down

Searching for information by drilling down has a fundamental limitation that is
set out formally in information foraging theory.[^2] Consider that the data
model is hierarchically structured data and the search involves following
information scent down a multi-way branching tree. Information scent is almost
always less than perfect and it has been shown that even with quite high
probability that information scent is accurate (e.g. $p = 0.7$) the search cost rise
exponentially with the depth of the search tree. This is set out formally in
Pirolli and Card.[^2] The branching factor is also a critical variable.

The equations are complex, but in simple terms this means that finding
information via hierarchical drill down will be extremely inefficient for high
depth searches with high branching factors. This is why key word searches are to
be preferred over drill down for large amounts of data. In the case where there
is a 70% chance that information scent is an accurate predictor, a 5 level
hierarchy will only result in the required information being found 16% of the
time by following the highest scent symbol at each level. In other cases much
longer searches through mostly irrelevant information nodes will result.

### The drill down epistemic action cost hierarchy

A key design issue in supporting drill down is choosing the method for revealing
additional information. The following is a sequence from low cognitive cost to
high cognitive cost. The low cost operations are relatively effortless, but
generally only show a little information. As a general principle, lower cost
methods are preferred over high cost methods, but only if they reveal
information adequate to the task.

**Eye fixation:** The most natural way of obtaining more information about a
visible entity is to fixate it. This causes the object to be imaged on the
fovea where more detail may be seen, if it is available. Eye fixation is not
normally considered a drill down operation;however, eye fixation is an
epistemic action to obtain information just as much as clicking on an object.
Eye fixations can allow for drill down operations executed at a rate of 3/sec.

**Mouse hover:** With a mouse hover query (or touch), simply moving a cursor
over a symbol causes additional information to be revealed without significant
lag. The information is displayed in a compact form as near as possible to the
symbol. Typically with a hover query only a single set of drill down
attributes is visible at a time. Hover queries can allow for drill operations
executed at a rate of 1/sec.

**Click to open, Click to close:** Click to open causes an information panel to
be revealed showing additional attributes of the entity. This can have the
form of a small linked rectangle, embedded in the display, or it can be
displayed in a side panel. Normally it takes an additional click to close the
drill down panel which allows for multiple panels to be simultaneously showed.

A perceptual issue with click to open is that the newly opened panel may obscure
the base visualization. If the panel is placed to the side, then a method should
be provided for linking the drill down information to the selected symbol. This
is important if several drill down panels can be open simultaneously.

A variant on click to close is keeping only the last $n$ panels open ($n \geq 1$).
This removes the need to close panels.

**Click to open new display window, replacing previous window:** The most
disruptive form of drill down is having a new screen containing the drill down
information, replace the original screen. Closing the new screen or using a
back button restores the original display.

### Perceptual and cognitive issues

Replacing the original screen with a new display window method causes a loss of
context and this places a burden on working memory if the new information must
be related to what was previously seen. The problem will be worse if many drill
down operations are carried out in sequence. Working memory limitations can make
it necessary to redo drill down operations many times.

------

### Related VTDPs
[VTDP Drill Down-Close Out with Hierarchical Aggregation](/drill-drown-close-out/)
 is a form of drill down
where data has been aggregated in a hierarchical structure.

There is a fine distinction between drilling down on an entity and following
links from an entity. For example, if the entity represents a person, drilling
down might reveal where they live where they have been, etc. But we might also
ask who they know and this involves following links to other entities
([VTDP Seed then Grow](/seed-then-grow/)).

------

### References

[^1]: Shneiderman, B. (1996) The Eyes Have It: A Task by Data Type Taxonomy for Information Visualizations. In Proceedings of the IEEE Symposium on Visual Languages, pages 336-343, Washington. IEEE Computer Society Press.

[^2]: Pirolli, P. (2009) Information Foraging Theory. Oxford Series in Human Technology Interaction.

[^3]: Hogg, T and Huberman, B.A. (1987) Artificial Intelligence and large scale computation: A physics perspective. Physics Reports, 156, 227-310.
