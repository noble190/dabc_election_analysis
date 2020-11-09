# Election Analysis

## Overview
The purpose of this election audit analysis is to review raw vote data, grouped by candidate and county, in order to neatly summarize the results of the election. 
The election summary includes:
* The total # of votes cast
* Votes broken down by county
* The largest county turnout
* Votes broken down by candidate
* The winning candidate

## Results

* There were a total of 369,711 votes cast in this election:

  * Jefferson County: 38,855 votes, 10.5% of the total
  * Denver County: 306,055 votes, 82.8% of the total
  * Arapahoe County: 24,801 votes, 6.7% of the total
  
* Denver county had the largest # of votes, at 82.8% of total votes

* Votes by candidate:

  * Charles Casper Stockham: 85,213 votes, 23% of the total
  * Diana DeGette: 272,892 votes, 73.8% of the total
  * Raymon Anthony Doane: 11,606 votes, 3.1% of the total
  
* The winner of the election is Diana DeGette, with 272,892 votes (73.8% of total votes)

## Summary
This script can be re-used for any other election with two minor modifications. As-is, it uses a hardcoded name for the election district - 'County', which may not be relevant for all elections. This script can easily be made more dynamic by reading the election district name from the data .csv file, instead.

This would require only two code changes:

1. Capture the election district name from the .csv header row, index of 1:
![Capture election district name from .csv header](https://github.com/noble190/dabc_election_analysis/blob/main/Resources/mod1.png)

2. Update any hardcoded references to 'County' in the script output to use the newly created variable:
![Update hardcoded election district names with references to the new election district variable](https://github.com/noble190/dabc_election_analysis/blob/main/Resources/mod2.png)

The above changes would result in a script that is applicable to a much wider range of elections.
