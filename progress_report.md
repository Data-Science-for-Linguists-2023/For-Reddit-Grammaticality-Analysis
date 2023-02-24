## Repository created 
### February 12, 2023
The repository for the term project has been created. Several files have been added to the repository, such as LICENSE.md, project_plan.md,
progress_report.md, README.md, and .gitignore. I have figured out which subreddits I would like to collect posts from, which are several
subreddits dedicated to various cities in the United States. I have registered my project with the Reddit API so that I can use the Reddit
API for my project.

## 1st Progress Report
### February 24, 2023

The 1st Progress Report revolved around the data that I will use for this project. The first thing that I did was read about and experiment 
with [PRAW](https://praw.readthedocs.io/en/stable/), the Python Reddit API wrapper that I used to collect posts and various information about posts. 
The Notebooks folder and the dataCollection were created to collect data on Jupyter Notebook. The next thing I did was select a variety of different subreddits that I believed would be good to analyze. I have switched from doing subreddits related to cities, as I agreed with the feedback that I received that the regional differences wouldn't be very noticeable in writing. Therefore, I have pivoted to the idea of different subreddits that would potentially exemplify the different ways people write, such as gamers, lawyers, and students. Once I selected a variety of subreddits, I used the API to read in posts from the subreddits into DataFrames. I decided to include information such as the title, the author, the text, the number of upvotes, the number of comments, and the ratio of votes. I cleaned these dataframes up through removing entries that had blank text. I read these dataframes into csv
files for data display purposes. It took about fifteen subreddits to reach my goal of >= 10,000 posts. I am not sure as to why the API didn't allow me
to read more than 900 posts from a subreddit at once, but that is something to look into. All of the data from the subreddits is saved into .csv files
in the data folder. A sample of this data can be found [here](https://github.com/Data-Science-for-Linguists-2023/For-Reddit-Grammaticality-Analysis/tree/main/data_samples). The data notebook can be found [here](https://github.com/Data-Science-for-Linguists-2023/For-Reddit-Grammaticality-Analysis/tree/main/notebooks).
#### Sharing Plan
Considering all of the data that I am using is publicly available on Reddit, I plan to make all of my data publicly available. Reddit only limits uses
in the case where it is commercial, which I do not intend to do. I will review the licensing information on Reddit before I make a final decision. If
it turns out I am wrong and I cannot make my data publicly available, if possible, I will try to post smaller samples to exemplify the type of data
that I worked with during this project.
