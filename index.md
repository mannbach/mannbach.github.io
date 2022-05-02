---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: "Jan Bachmann"
---
Hi there! I am a PhD student at [Complexity Science Hub](https://csh.ac.at) in Vienna and the [Department of Network and Data Science](https://networkdatascience.ceu.edu/) (DNDS) of [Central European University](https://www.ceu.edu/). Computer Science graduate of [RWTH Aachen University](https://rwth-aachen.de) and [FH Aachen University](https://fh-aachen.de).

In my research I study how inequalities between a minority and majority group can emerge from local collaboration behavior.
My projects center around temporally evolving collaboration networks, rank dynamics and the occasional fairness concerns of modern network based AI algorithms.
All of these projects are within the awesome [Network Inequality Group](https://networkinequality.com/) lead by [Fariba Karimi](https://www.csh.ac.at/researcher/fariba-karimi/) ✌️

Beyond my research interests, I am very passionate about bouldering, hiking, and the good ol' books and movies.
Feel free to shoot me a message in case you want to discuss any of my research, or anything else really.
## Events
__2022-05-11__: PhD Proposal Defense at the weekly research seminar at DNDS [🗓](events/22-05-11_proposal_defense.ics) (_please contact [me](mailto:jan@mannbach.de) in case you want to attend_)

## Posts
{% for post in site.posts %}
#### {{ post.date | date: "%Y-%m-%d" }} [{{ post.title }}]({{ post.url }})
{{ post.excerpt }}
{% endfor %}

## Publications
- __Jan Bachmann__. "Measuring Temporal Dependencies in Music Listening Behavior across Countries." [Master Thesis](https://drive.google.com/file/d/1fvGMRu4D), August 27, 2020.
- Schumacher, Tobias, Hinrikus Wolf, Martin Ritzert, Florian Lemmerich, __Jan Bachmann__, Florian Frantzen, Max Klabunde, Martin Grohe, and Markus Strohmaier. “The Effects of Randomness on the Stability of Node Embeddings.” [ArXiv:2005.10039](http://arxiv.org/abs/2005.10039) [Cs, Stat], May 20, 2020.
