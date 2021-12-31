# Election-Analysis

## Overview of Election Audit

A Colorado Board of Education employee has given us the following tasks to complete the election audit of a recent local congressional election. The purpose of this project is to compile this data in a manner that is concise and accurate for the election commission. Python language was used for the analysis which was sourced from elections_results.csv. Python was used specifically so that we could create a script that performs complex mathematical operations, utilizes modifiable for-loops and conditional statements, and is able to then be printed to a shareable text file. In doing so, the election commission can view the summary of the election analysis results in a readable format.

1. Calculate the total number of votes cast.
2. Get a complete list of candidates who received votes.
3. Calculate the total number of votes each candidate received.
4. Get a complete list of counties where voters resided in.
5. Calculate the total number of votes each county accounted for.
6. Calculate the percentage of votes each candidate won.
7. Calculate the percentage of votes each county accounted for.
8. Calculate the largest county vote turnout.
9. Determine the winner of the election based on popular vote.

## Resources

* Data Source: election_results.csv
* Software: Python 3.6.1, Visual Studio Code, 1.38.1

## Election-Audit Results

The candidate analysis of the election shows that:
* There were 369,711 votes cast in the election.
* The candidates were:
    * Charles Casper Stockham
    * Diana DeGette
    * Raymon Anthony Doane
* The candidate results were:
    * Charles Casper Stockham received 23.0% of the vote and 85,213 number of votes.
    * Diana DeGette received 73.8% of the vote and 272,892 number of votes.
    * Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes.
* The winner of the election was:
    * Diana DeGette, who received 73.8% of the vote and 27,2892 number of votes.

The county analysis of the election shows that:
* The county turnouts were:
   * Jefferson county accounted for 10.5% of the vote and 38,855 of votes.
   * Denver county accounted for 82.8% of the vote and 306,055 of votes.
   * Arapahoe county accounted for 6.7% of the vote and 24,801 of votes.
* The largest county turnout of the election was:
   * Denver, which accounted for 82.8% of the vote and 306,055 of votes.


<img src="https://github.com/katmarcin/election-analysis/blob/b7c6b41abd901caa231c0bd8c2231dce01988d24/Election_Analysis.png" width="450" height="450">
   

## Election-Audit Summary

Dear Election Commission,

The script used to analyze the election results data can be applied with modifications to other elections of various scales or to data that has more subcategories. The template is a great foundation for further analysis to allow for the election commission to provide accurate conclusions from electoral review. Without a supportive script, this would be a lengthy and costly process. A well-built script allows one to quickly analyze any electoral dataset for which examples are provided below:

1) This election audit analysis simply focuses on county turnout and candidate results. However, if the election commission wishes to analyze the breakdown of either the county or candidate votes by demographic such as voting party, it may lead to a better understanding of where candidates succeeded more than others. In this scenario, we could use "Democrat", "Republican", and "Independant" as our fourth column in the election_results.csv dataset. First, to obtain the party data you would create a party options list and party votes dictionary, then establish variables for largest party turnout. Largest party vote is initialized at zero. Party name is extracted in similar fashion as the other categories and an if-statement coupled with a not-in operator is used to add a party name to the party list, if it does not match any existing one. Second, a for-loop is established to get the party from the party dictionary and calculate the percentage of votes that each particular party accounted for. Most importantly, an f-string formatted print statement is used to then save the party results to the text file so that it can be utilized for the review. These same methods can practically be applied to any type of demographic as long as it is recorded in the dataset. Other examples may include gender or race.

2) The dataset we used in this analysis hones in on county vote specifics as it relates to a state's congressional turnout. However, if we wanted to apply this script to a smaller scale, such as city official elections, we would simply replace "county" with an electoral subdivision such as a "ward". Wards are used commonly in large city elections for representative purposes. For example, the city of Houston, Texas has six wards which can be used to review election data. Using our template, we can replace any variable or statement which says "county" and replace it with "ward". The respective names of those wards can be listed as "First Ward, Second Ward, etc..." in any column location within the dataset. This audit analysis would allow us to view any trends related to ward turnout or popularity with a particular candidate. 

Simply put, this is an exceptional script that can be used for a variety of election data analyses that allows you to analyze a large number of categories and can be modified with relative ease to produce a proper summary of desired information.
