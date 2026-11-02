# S2PGAGOLF
DS2023 Final Project on PGA Golf EDA


## Main Collaborators:
Sahil Sardar, Austin Genova, Will Chappell, Conner Elling, Ben Chapuis


## High-Level Research Questions (Task Level)
1) Which golf skills most strongly drive scoring success on the PGA Tour?
2) How does an individual player’s performance compare to other players and to the tour overall?
3) How have player performance and the average playing style as well as winning play style/strategy changed from 2015 to 2022?
4) What factors are associated with a player’s tournament results and earnings?
5) How do players with similar scoring success differ in the way they achieve their scores?

## Mid-Level Questions (Sub-task Level)
For each high-level research question:

1)
* Which strokes gained category (off the tee, approach, around the green, putting) has the strongest relationship with scoring average?
* Do the skills that separate top-10 finishers from the rest of the field differ from the skills that matter for the average player?
 
2)
* In which skill categories is a selected player above or below the tour average?
* Which players have a performance profile most similar to a selected player’s?
 
3)
* How have averages across the tours for driving distance and driving accuracy changed from season to season? Are they constantly rising?
* Which seasons did a chosen player’s performance rise or drop drastically compared to their regular performance level?
 
4)
* Which statistics are most strongly associated with higher season earnings?
* Do the factors linked to earnings change from one season to another?
 
5)
* When looking at players with similar scoring averages, which ones make noticeably less pars than their peers?
* Among higher performing players, who relies more on birdies and who relies more on avoiding bogeys?

## Low-Level Questions (Operation Level)

1)
* 1a: Which strokes gained category has the strongest relationship with scoring average?
Action: Correlate. Target: each strokes gained category against scoring average.
Then Find extremum on the resulting correlation values to pick the strongest.
* 1b: Do the skills separating top-10 finishers from the rest differ from those that matter for the average player?
Action: Filter (top-10 vs. rest), then Characterize distribution of strokes gained. Target: each strokes gained category within each group.
Compare the two groups’ distributions.

2) 
* 2a: In which skill categories is a selected player above or below the tour average?
Action: Retrieve value (player’s stats), then Compute derived value. Target: tour average per category, then the gap between player and average.
* 2b: Which players have a profile most similar to a selected player’s?
Action: Compute derived value (a similarity or distance score), then Sort. Target: all players’ skill profiles ranked by closeness to the selected player.

3) 
* 3a: How have tour-wide averages for driving distance and accuracy changed by season?
Action: Compute yearly mean, then Correlate (or describe the trend). Target: driving distance and accuracy across seasons.
* 3b: In which seasons did a selected player rise or drop sharply versus their own typical level?
Action: Retrieve value (player’s seasons), then Find anomalies. Target: the player’s season-to-season performance values.

4)
* 4a: Which statistics are most strongly associated with higher season earnings?
Action: Correlate, then find extremum. Target: each statistic against season earnings.
* 4b: Do the factors linked to earnings change from season to season?
Action: Filter (by season), then Correlate. Target: statistics against earnings within each season, then compare across seasons.
5) 
* 5a: Among players with similar scoring averages, which make noticeably fewer pars?
Action: Filter into tiers of scoring averages(potentially through clustering), then find anomalies and outliers in their scoring variance. Target: par frequency within that group.
* 5b: Among high , who relies more on birdies versus avoiding bogeys?
Action: Filter (high performers), then Compute derived value (birdie-to-bogey balance), then Sort. Target: each player’s birdie and bogey rates.
