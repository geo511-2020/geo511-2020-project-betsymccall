District Maps: Does geometric compactness make a district more fair?
================

# Introduction to problem/question

# Problem / Question

Gerrymandering (the art of making a district map unfair) is a
well-established practice, but what features makes a district map fair?

# Inspiring Examples

Gerrymandering has been going on in district map design since before the
Republic. People that draw maps to gain advantage have several
techniques for creating biased districts, such as cracking (splitting up
the constituencies of minority parties across multiple districts to
minimize their impact) and packing (putting more of a constituency in a
single district to run up the score there and blunt their impact in
other districts). But the properties of districts that make district
maps more fair has had very little research. Features like compactness
have been proposed, with various definitions, but the research to
establish this as a viable marker of fairness has not really been done.

The example below is a map of Congressional races from 2018. The first
thing to do is to recreate a similar map for each election year to be
analyzed. My goal would be to colorize by margin of victory, which could
suggest which states are highly gerrymandered: one highlight would be
small margins of victory in the party that took the majority of seats,
and the minority party winning in their districts by much larger margins
(sign of cracking and packing).

## Example 1

![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/US_House_2018.svg/480px-US_House_2018.svg.png)

This district map shows gains and losses, which isn’t quite what I have
in mind, but close enough.

## Example 2

![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/49/116th_US_Congress_House.svg/450px-116th_US_Congress_House.svg.png)
Another way to display districts in a map would be to compare the
state-wide election results (what percent of the state voted for members
of Congress in a particular party) vs. the number of seats they won in
state Congressional delegation.

For example: in Ohio in 2018, Ohioans voted for Republican members of
Congress at 51%, and Democrats at around 48% (the rest third party).
But, the GOP won 12 of 16 (75%) of the Congressional delegation. This
would be a strong indicator of an unfair district map. In a fair map,
you should expect the percentages to be more similar (give or take an
integer number of seats).

# Proposed data sources

[United States Congressional District
Shapefiles](http://cdmaps.polisci.ucla.edu/)

![](http://cdmaps.polisci.ucla.edu/png/congdist028.png)

[MIT Election Data](https://electionlab.mit.edu/data) The shapefiles go
back to 1789, but MIT’s data appears to go back to only 1976. Still 1976
is more than 20 Congressional election cycles.

# Proposed methods

First, merging the data requires quite a bit of pre-processing. Aside
from the proposed maps, I would like to calculate some features from the
shape files such as area, perimeter, compactness (perhaps more than one
version), and use regression and classification methods to determine if
any of the selected features has a predictive relationship with a more
representative Congressional delegation outcome. Indeed, we could
compare the predictions based on data through 2018 (MIT’s data seems to
start in 1976), to the predict the outcomes from 2020, and see if they
agree. States with only one Congressional district will also have to be
excluded.

# Expected results

Want to produce some maps for visual comparison, and to determine if
compactness (for instance) has any relationship to predicting fairer
outcomes.
