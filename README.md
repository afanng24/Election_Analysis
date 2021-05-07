# Written Analysis of the Election Audit 

## Overview of Project
For this project a Colorado Board of Elections employee, Seth, has asked for help in completing an election audit of a recent local congressional election. Seth has asked for the following tasks to be completed:
- Calculate the total number of votes cast.
- Get a complete list of candidates who recieved votes.
- Calculate the total number of votes each candidate recieved.
- Calculate the percentage of votes each candidate won.
- Determine the winner of the election based on popular vote. 

All of which was accomplished under the "PyPoll.py" python file. Additionally the election commission has also requested:

- The voter turnout for each county
- The percentage of votes from each county out of the total count
- The county with the highest turnout

All of which is contained within the “PyPoll_Challange.py '' Python file and the results of which could be easily read in the election_analysis.txt. Furthermore, the methods used to create the additional information and the difference between the two Python files will be included towards the end of the analysis under "Explaining the Code and Introductions."


## Resources
**Source of Data** : election_results.csv

**Software** : Python 3.7.6 , Visual Studio Code.

## Election-Audit Results
The results of the election is as follows:

369,711 total votes were cast in this congressional election.
- Number of votes and the percentage of total votes for each county:
  -   Jefferson County had 10.5% of the votes for a total of 38,855 individual votes.
  -   Denver County had 82.8% of the votes for a total of 306,055 individual votes.
  -   Arapahoe County had 6.7% of the votes for a total of 24,801 individual votes.


In summary Denver County had the largest number and percentage of votes.

- The candidates and their share of the vote:
  - Charles Casper Stockham recieved 23.0% of the vote with 85,213 individual votes.
  - Diana Degette recieved 73.8% of the vote with 272,892 individual votes.
  - Raymon Anthony Doane recieved 3.1% of the vote with 11,606 individual votes.


Diana Degette won the election with 272,892 individual votes and 73.8% of the total vote. 



  
## Election-Audit Summary

The code provided in PyPoll_Challanges can be formatted based on information contained in its attached csv file. The file currently includes candidates, votes, and counties that voted. If the file were to be expanded with additional information then there is no reason it can’t be used for a plethora of other elections ranging from local elections, mayoral elections and even presidential elections. For mayoral elections one might include districts and the total number of people who voted in their respective districts, the code in PyPoll_Challanges could then be formatted to district_name, district_percentage, and district_results so on and so forth. As long as the district votes were on the same row of the csv file. 
If this code were to be used in a presidential election that would include both county and state votes then a state dictionary would be made just as the county dictionary was made. Depending on what row the state votes are on, the information could be pulled from that csv file and included into the python code. This would give the same information that was collected from county votes to state votes as well. All of which would then be formatted and read easily in the election_analysis.txt attached in the Elections_analysis folder. 



## Explaining the Code and Introductions

This section is an addition created to further explain the code and why some lines of code are used. This will make it easier to review further down the line should anyone ever need to revisit syntax or misunderstand what certain lines accomplishes. The challenge itself is called "PyPoll_Challange.py" while the homework file was named "PyPoll.py" much of the challenge is simply restructuring what we have learned in "PyPoll.py" and making it work in the challenge file. Screenshots will be added where it is necessary. 


## Instuctions 
-      1: Create a county list and county votes dictionary.
-      2: Track the largest county and county voter turnout.
-      3: Extract the county name from each row.
-      4a: Write an if statement that checks that the county does not match any existing county in the county list.
-      4b: Add the existing county to the list of counties.
-      4c: Begin tracking the county's vote count.
-      5: Add a vote to that county's vote count.     
-      6a: Write a for loop to get the county from the county dictionary.
-      6b: Retrieve the county vote count.
-      6c: Calculate the percentage of votes for the county
-      6d: Print the county results to the terminal.
-      6e: Save the county votes to a text file.
-      6f: Write an if statement to determine the winning county and get its vote count.
-      7: Print the county with the largest turnout to the terminal.
-      8: Save the county with the largest turnout to a text file.
 
 ## Code and Comparisons
 
 ### 1: Create a county list and county votes dictionary.
 
 The easiest part, creating a dictionary for the county names and county votes they are named county_names and county_votes respectfully which mirrors the first lines of code in PyPoll.py where we had to create candidate options and candidate votes. 
### PyPoll
![PyPoll1](https://user-images.githubusercontent.com/82983000/117485441-5f7c2b80-af36-11eb-8131-c0b275dfd061.png)
### PyPoll Challenge
![PyPollChallange1](https://user-images.githubusercontent.com/82983000/117485603-8e929d00-af36-11eb-9672-7fd9b37fc876.png)

### 2: Track the largest county and county voter turnout.
Since there is no percentage yet, PyPoll Challange only needs to track largest county turnout and largest county vote which is named largest_county_turnout and largest_county_vote respectfully. 
### PyPoll
![PyPoll2](https://user-images.githubusercontent.com/82983000/117486026-1d9fb500-af37-11eb-8997-7d4e9bb6c86b.png)
### PyPoll Challenge
![PyPollChallange2](https://user-images.githubusercontent.com/82983000/117486056-26908680-af37-11eb-8a41-db99d2696e09.png)
### 3: Extract the county name from each row.
Inserting county_name from the file, note that it is important to do this under the for - in row just like the candidate_name above this line. The excel file has the name of each county in the second row so since it starts with 0 the county names would be under [1]. 
### PyPoll Challenge
![PyPollChallange3](https://user-images.githubusercontent.com/82983000/117486487-b6cecb80-af37-11eb-9b2f-9bc3c8c776c8.png)
### 4a - 4c: Write an if statement that checks that the county does not match any existing county in the county list. Add the existing county to the list of counties. Begin tracking the county's vote count.
4a - 4c was introducing the newly created dictionaries to the code and followed from the PyPoll excersie when we had to do the same for the candidate votes and candidate names. 
### PyPoll
![PyPoll4](https://user-images.githubusercontent.com/82983000/117487003-73289180-af38-11eb-8e8f-3555a7fb216d.png)
### PyPoll Challenge
![PyPollChallenge4](https://user-images.githubusercontent.com/82983000/117487015-79b70900-af38-11eb-9e56-b5454113afa7.png)
### 5: Add a vote to that county's vote count. 
Same idea as instruction 4. 
### PyPoll Challenge
![PyPollChallenge5](https://user-images.githubusercontent.com/82983000/117487125-ad922e80-af38-11eb-9e59-a69ea1fc1b71.png)
### 6a - 6f 
Same principle as the other PyPoll code however this section took the longest, specifically 6c where we had to calculate county percentage. The original code had float(votes/float(total_votes) * 100 to find the percentage however float wouldn't work with the county vote. Precision was needed for vote percentage hence the float function, the interger function was used for the county percentage instead. 
6f was also a deviation from the original code as we only needed to find the winning county and its turnout as opposed to needing to figure out the vote count, percentage, and candidate. The original code had an IF - AND statement whereas the challenge colde just needed an IF statement without the and.  

### PyPoll
![PyPoll6](https://user-images.githubusercontent.com/82983000/117488202-1e861600-af3a-11eb-9a13-3010e06848ab.png)
### PyPoll Challenge
![PyPollChallenge6](https://user-images.githubusercontent.com/82983000/117488217-234aca00-af3a-11eb-9236-7160e8468935.png)
### 7: Print the county with the largest turnout to the terminal.
Same code as PyPoll.py but since only the Largest County Turnout was needed only one f string with words were needed, the rest were dashed lines to separate the rows and largest_county_turnout outcome was inserted into the {} brackets. 
### PyPoll
![PyPoll7](https://user-images.githubusercontent.com/82983000/117489400-96087500-af3b-11eb-868c-80b948089afb.png)
### PyPoll Challenge 
![PyPollChallegne7](https://user-images.githubusercontent.com/82983000/117489417-9b65bf80-af3b-11eb-94f6-0ff74d885e40.png)
### 8: Save the county with the largest turnout to a text file.
Ending the code by saving the final largest county turnout into the textfile, instead of putting winnging_candidate_summary into the textfile (which comes later in the challenge code) we insert largest_county_turnout which writes it down in the textfile. 
### PyPoll
![PyPoll8](https://user-images.githubusercontent.com/82983000/117490011-44141f00-af3c-11eb-9795-355b345ff756.png)
### PyPoll Challenge 
![PyPollChallegne8](https://user-images.githubusercontent.com/82983000/117490023-48d8d300-af3c-11eb-98f9-fdf2e41ad1bf.png)





