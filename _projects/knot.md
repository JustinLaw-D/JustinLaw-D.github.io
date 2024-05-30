---
layout: page
title: Knot Groups
description: Symmetries, Representations, and Pretty Graphs
img:
importance: 1
category: Work
pdf : KnotGroupReps.pdf
---

This page is mostly an excuse to show off something cool I made during my summer working with <a href = 'https://personal.math.ubc.ca/~tbjw/'>Ben Williams</a> that wouldn't show up in the paper. At one point during the summer, I was studying how the symmetries of <a href = 'https://knotinfo.math.indiana.edu/diagram_display.php?9_48'>knot 9-48</a> act on its corresponding fundamental group. Generally the way you do this is quite geometric, just draw out the generating loops of the fundamental group and see where they end up under the symmetric transformation. The issue is that this doesn't work with <a href = 'https://knotinfo.math.indiana.edu/diagram_display.php?9_48'>knot 9-48</a>, as there are no symmetries of the knot that can be seen in $$\mathbb{R}^3$$ alone. We instead need to work with $$\mathbb{R}^3$$ with an added point at infinity, and symmetries that look like this.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/symmetry.gif" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A visualization of a torus transforming under symmetries in \(S^3\) which are not present in \(\mathbb{R}^3\).
</div>

My solution to this was simple, but very time-consuming: Create a 3d graphing program which plotted surfaces and curves projected into $$\mathbb{R}^3$$ from $$S^3$$, using coordinates for $$S^3$$, and use these coordinates to more easily apply the required transformations. The early tests of this were with a much simpler <a href = 'https://knotinfo.math.indiana.edu/diagram_display.php?5_1'>(5,2)-torus knot</a>.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/torus.gif" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

After this, I applied the program to <a href = 'https://knotinfo.math.indiana.edu/diagram_display.php?9_48'>knot 9-48</a> with an extra rotation about the z-axis.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/948.gif" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Using this, I was able to determine the action of this transformation on the corresponding knot group for <a href = 'https://knotinfo.math.indiana.edu/diagram_display.php?9_48'>knot 9-48</a>. If you're interested in the gritty details (along with all the rest of the calculations I did that summer) see the pdf at the top of the page.

I'll end this off with a couple of links. <a href = 'https://www.geogebra.org/m/uknpwksx'>The finished product for knot 9-48</a>, and <a href = 'https://www.geogebra.org/m/nsxjpwnu'>a template for those of you crazy enough to try and do something like this yourself.</a> The plan that summer was actually to apply this again to ten crossing knots, but there didn't end up being enough time for it.