---
layout: post
title: Productivity Puzzle
---
For the a visualization class at [DNDS](https://networkdatascience.ceu.edu/) I studied the disparity between female authorships and active scientists in journals of the [American Physical Society](https://journals.aps.org/) (APS).

In this project used a dataset of APS publications for which the gender of the author had been inferred based on their first names.
Refer to [1] for details on the inference process.
An authorship is defined by a scientist (co-)authoring a publication in one of the APS journals.
I compute the share of female authorships of a given month as `f_auth = N_fem_auth / N_auth`.

Comparing the share of female authorships to how many scientists are active in a given month puts the fraction to perspective.
To this end, I mark a scientist as active in a given month if the month is between that scientist's first and last publication month across the entire dataset.
This allows me to compute the share of active female scientists in each year as `f_active = N_fem_active / N_active`.

The Productivity Puzzle describes the observation that female authors publish fewer papers (per author), an effect that can be accounted for by considering career age.
Here, I visualize this effect by computing the difference `df = f_auth - f_active` and animate its development through time (min/max rescaled):

![Temporal evolution of difference between share of female authorships and active scientists](/images/1990-to-end.gif)

A value of `df < 0.5` indicates that the share of female authorships in that year was lower than the share of active scientists which is the case for most of the present months.
To get a more complete picture, I plot the same value (without rescaling) as a heatmap:

![Heatmap of temporal evolution of difference](/images/heatmap_t.svg)

The presence of the Productivity Puzzle effect becomes obvious, indicated by the predominantly blue tiles.
Moreover, this development has become more consistent through time!
That is, the patterns are more mixed in early years (which could be due to random fluctuations caused by small sample sizes), but then moves to mostly negative values in later years.
So, the effect is not mitigated, but rather consolidated through time.

__Note__ that this analysis is more of an exploratory kind.
That is, it does not uphold to scientific standards, but merely serves as motivation for further and more rigorous studies in that direction.

## References
1. Kong, Hyunsik, Samuel Martin-Gutierrez, and Fariba Karimi. “First-Mover Advantage Explains Gender Disparities in Physics Citations.” [ArXiv:2110.02815](http://arxiv.org/abs/2110.02815) [Physics], October 6, 2021.
