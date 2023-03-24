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
The [notebooks/](https://github.com/Data-Science-for-Linguists-2023/For-Reddit-Grammaticality-Analysis/tree/main/notebooks) folder and the dataCollection notebook were created to collect data for this project. The next thing I did was select a variety of different subreddits that I believed would be good to analyze. I have switched from the idea of doing subreddits related to cities, as I agreed with the feedback that I received that the regional differences wouldn't be very noticeable in writing. Therefore, I have pivoted to the idea of different subreddits that would potentially exemplify the different ways people write, such as gamers, lawyers, and students. Once I selected a variety of subreddits, I used the API to read in posts from the subreddits into DataFrames. I decided to include information such as the title, the author, the text, the number of upvotes, the number of comments, and the ratio of votes. I cleaned these dataframes up through removing entries that had blank text. I read these dataframes into csv
files for data display purposes. It took about fifteen subreddits to reach my goal of >= 10,000 posts. I am not sure as to why the API didn't allow me
to read more than 900 posts from a subreddit at once, but that is something to look into. All of the data from the subreddits is saved into .csv files
in the data folder. In any case, the notebook took an extremely long time to run as the calls to read in the posts were very time consuming, which may be due to the way I read them in. I should see if there is anything I can do to speed that up in case I need to read in posts again. A sample of this data can be found [here](https://github.com/Data-Science-for-Linguists-2023/For-Reddit-Grammaticality-Analysis/tree/main/data_samples). The data notebook can be found [here](https://github.com/Data-Science-for-Linguists-2023/For-Reddit-Grammaticality-Analysis/tree/main/notebooks).
#### Sharing Plan
Considering all of the data that I am using is publicly available posts on Reddit, I plan to make all of my data publicly available. Reddit only limits uses in the case where it is commercial, which I do not intend to do.I will review the licensing information on Reddit before I make a final decision. If
it turns out I am wrong and I cannot make my data publicly available, if possible, I will try to post smaller samples to exemplify the type of data
that I worked with during this project. If I cannot do this, then I will create fake posts to exemplify how I worked with the data on this project, such
as annotations

## 2nd Progress Report
### March 23, 2023

The 2nd Progress Report revolved around data organization and analysis. The first thing that I did was create a second notebook, [dataOrganization.ipynb](https://github.com/Data-Science-for-Linguists-2023/For-Reddit-Grammaticality-Analysis/blob/main/notebooks/dataOrganization.ipynb). In this notebook, my goal was to combine the several .csv files that were generated from the first notebook, [dataCollection.ipynb](https://github.com/Data-Science-for-Linguists-2023/For-Reddit-Grammaticality-Analysis/blob/main/notebooks/dataCollection.ipynb). The reason for this is because the API is limited to 1000 posts per call, and I am working with a quantity of posts way larger than that. Therefore, I had to query subreddits multiple times, with sometimes having to wait for a few hours later, in order to get more posts. Once the .csv files were combined into one post, I then cleaned up columns and made all of the dataframes the same size. I found that the highest number that all of the subreddits could be, which is 1500. Therefore, each subreddit is now a collection of 1500 posts. At the end of this notebook, I packaged them up into .csv files for further use. The second thing that I did was create a third notebook, [dataAnalysis1.ipynb](https://github.com/Data-Science-for-Linguists-2023/For-Reddit-Grammaticality-Analysis/blob/main/notebooks/dataAnalysis1.ipynb). In this notebook, I used the [language-tool-python](https://pypi.org/project/language-tool-python/) as a base assessment for grammaticality. This included finding the top errors across subreddits, analyzing thoses errors, and comparing those errors between subreddits. This Progress Report taught me a lot about how huge data collection, organization , and analysis is. If I wasn't spending time figuring out how to do a specific task, I was copying the same task 15 times for each subreddit and letting it run.
#### Sharing Plan
For the found portion of my data, I will be making all of my data publicly available. Reddit's rules for the API are [here](https://docs.google.com/forms/d/e/1FAIpQLSezNdDNK1-P8mspSbmtC2r86Ee9ZRbC66u929cG2GX0T9UMyw/viewform). Within this webpage, Reddit outlines that posts can be displayed and formatted. Therefore, I am free to post samples of my data, which is csv files with information relating to Reddit posts.
#### Repository License Plan
