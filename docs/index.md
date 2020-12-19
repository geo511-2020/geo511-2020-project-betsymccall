What Makes a District Map Fair?
================
Betsy McCall

# Introduction

Gerrymandering has been going on longer than the Republic, and long
before there was a name for it. District maps are drawn by those in
power to maintain that power. Preserving incumbency has always been an
important motivator, and with the rise of political parties, maintaining
party control is also important to the legislatures drawing the maps.
Various methods have been developed, including cracking and packing, to
produce the legislature’s desired results. But while those in power are
happy with this situation, voters would prefer fair maps that were
capable of reflecting the preferences of the voters, including as they
change from election to election. But the methods to thwart
gerrymandering have had almost no research to determine what actually
works. Some methods like compactness, have been proposed, but even
researchers in the field note in the literature this gap in their
knowledge even as they design technical solutions for creating maps. The
goal here, therefore, will be to examine the fairness of current
district maps and to determine if compactness could be a viable solution
to the fairness question.

# Materials and methods

This project will rely primarily on data from two sources:

[United States Congressional District
Shapefiles](http://cdmaps.polisci.ucla.edu/) and [MIT Election
Data](https://electionlab.mit.edu/data).

The Congressional district shape files go back to 1789. MIT’s election
data seems to only go back to 1976, but this will be enough for an
initial start. From the shapefiles we can calculate area and perimeter
of the districts which will go into our calculation of compactness. We
can probably also use the area of the districts as a proxy for relative
density since Congressional districts have to have about the same number
of seats during the time period to be considered. The election data will
have to be joined to the shapefiles to determine the winners of the
elections.

Maps can be produced compare the statewide winning party (based on vote
totals), and compared to the outcomes by seats in the Congressional
delegation to determine how closely (or not) that they align. A larger
deviance, would suggest worse gerrymandering.

And finally, classification and regression methods will be employed to
determine if some of the proposed definitions for compactness actually
correlate to fairer district outcomes.

Code: Working on it\!

Data: Available in the links above.

Here’s my first code chunk.

R code will come later. All hiding now.

## Download and clean all required data

Add any additional processing steps here.

# Results

Coming soon\!

# Conclusions

coming soon

# References

All sources are cited in a consistent manner [Project
Proposal](http://betsymccall.net/edu/CDSE/coding/R/Project_Proposal.html)
