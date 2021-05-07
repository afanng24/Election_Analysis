# Explaining the Code

## Introduction

This Readme is not a part of the challenge but rather a personal addition created to further explain the code and why some lines of code are used. This will make it easier to review further down the line should I ever need to revisit syntax and forget what some lines accomplishes. The challenge itself is called "PyPoll_Challange.py" while the homework file was named "PyPoll.py" much of the challenge is simply restructuring what we have learned in "PyPoll.py" and making it work in the challenge file. I will add screenshots where it is necessary. 


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
 
 The easiest part, creating a dictionary for the county names and county votes they are named county_names and county_votes respectfully which mirrors the first liens of code in PyPoll.py where we had to create candidate options and candidate votes. 
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
![PyPollChallange3](https://user-images.githubusercontent.com/82983000/117486487-b6cecb80-af37-11eb-9b2f-9bc3c8c776c8.png)




 
 
