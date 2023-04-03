---
date: 2023-04-03
title: Mean Reversion
categories:
  - examples
author_staff_member: gene
excerpt_separator: <!--more-->
---

##  Buy the Dips NASDAQ
Lets try a strategy where we buy the dips for NASDAQ. What do we count as a dip? Lets say If the 5 day cumulative return is less than -5%. If there is a dip, lets by TQQQ, a 3x leaverages version of NASDAQ. lets also make sure we are not coming out a dip, or if the 1 day return is less then 5%. To do this, we insert a nested If/Else statement inside another If/Else statement to combine the two conditions. For the Else condition, we can leave empty, to just hold cash and do nothing.

![Checkmate]({{ site.baseurl }}\images\nasdaqdip.PNG){: .screenshot}

## Does it work?
wow! this strategy is on par with NASDAQ itself, and even narrowly beating out S&P 500 from the years 2015-2022, while only holding TQQQ a tiny percentage of the time, as we can see from the performance graph. This strategy is based on the idea of mean reversion, which states that a price has a tendancy to revert to its mean, after a big movement, like a dip.

![Checkmate]({{ site.baseurl }}\images\dips2.PNG){: .screenshot}
<!--more-->