# election-analysis
Analyze election results using Python

### Table of Contents
- [1 Purpose](#1-purpose-of-election-analysis)
  - [1.1 Required Tools](#11-required-tools)
- [2 Election-Audit Results](#2-election-audit-results)
- [3 Election-Audit Summary](#3-election-audit-summary)

## 1 Purpose of Election Analysis
 
The purpose of this analysis was to assist a Colorado Board of Elections employee, Tom, in an election audit of tabulated results for U.S. Congressional Precinct in Colorado using Python to automate the process. Tom had requested to view the following information derived from the data: 

- Total number of votes
- Number of votes received for each candidate
- Percentage of votes received for each candidate
- Overall winner of the election 

Given that the results of this coding script were successful, the code generated for this analysis can be used to audit other congressional districts, senatorial districts, and local elections. 

### 1.1 Required Tools

- Python 3.7.6
- Visual Studio Code or equivalent text editor
- Microsoft Excel version 16 or newer

## 2 Election-Audit Results

### 2.1 Number of Votes Cast in the Congressional Election 

Based on the election analysis csv file and the image below, **369,711** votes were cast in the Congressional election:

![](images/total_votes_cast.png)

To get the total number of votes cast using Python, the following code snippets were used to:
  1. Initialize the total vote counter and set it to **zero**
 
````total_votes = 0````

  2. Iterate through each row of the CSV file and add **one** vote for each row
  
````total_votes = total_votes + 1````

  3. Print results to the terminal and save to the election analysis text file

````with open(file_to_save, "w") as txt_file:````

````
election_results = (

f"\nElection Results\n"

f"-------------------------\n"

f"Total Votes: {total_votes:,}\n"

f"-------------------------\n\n"

f"County Votes:\n")
````

````print(election_results, end="")````

````txt_file.write(election_results)````


### 2.2 Breakdown of Number of Votes and Percentage of Total Votes for Counties in the Precinct

To find the number of votes derived from each county

## 3 Election-Audit Summary
