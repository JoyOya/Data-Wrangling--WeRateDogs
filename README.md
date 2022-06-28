# Data-Wrangling--WeRateDogs
This is Udacity DANA Project on WeRateDogs
Analyzing tweet archive  of a twitter account "WeRateDogs" --that rates people's dogs with a humorous comment about the dog.

WeRateDogs is a tweeter account that rates people’s dogs based on their pictures, videos, breeds and names. These ratings where gathered, cleaned, assessed and visualized. 
Three data source where gathered to achieve this report. This was how the report where gotten

1.	*Gathering of Data*

a.	The first file is the (twitter_archive_enhanced.csv). 
b.	The second one was the (image_predictions.tsv).  this file was downloaded programmatically using my request library and URL code that was provide by Udacity
c.	The third file was, tweet_json.txt and twitter_api.py, which was downloaded from the link provided in my Udacity classroom.
After gathereding these files, It was uploaded to a Jupiter notebook and the libraries were imported.

2.	*Assessing Of Data*

The three data was assessed both visually and programmatically to check for quality and tidiness issues. I then went ahead to  detect and document  eight (8) quality issues and two (2) tidiness issues in the "Accessing Data" section in the wrangle_act.ipynb of my Jupiter Notebook
Here are some of the quality and tidiness issues I assessed

3. *Quality Issues*

1. They were some incorrect datatypes on tweet_id and time stamps
2. They were 181 entries in (retweeted_status_id, reweeted_status_user and reweeted_status_timestamp) instead of 2356 entries 
3. They were 78 entries in (reply_to_status_id and reply_to_user_id) making it to have about 2278 missing entries.
4. The expanded_urls had some missing values too. It had just 2297 entries instead of 2356 
5. Some of the breeds of the dogs where not properly capitalized in p1, p2 and p3. 
6. Some of the tweets where retweeted, making must of them not original tweets
7. Some of the tweets had missing images 
8. Both the rating_numerator and rating_denorminator had incorrect ratings
9. Some of the tweets in the name column valid name

4. *Tidiness Issues*

1. The three different data set had one (1) common column, which is "tweet_id"   they all need to be   merged and put in just one dataset.
2. There are four different columns for dog names (doggo, floofer, pupper and puppo) and they ought to be put in a single column

5.	*Cleaning of Data*

Firstly copies of each of the following data files (twitter_archive_enhanced.csv, image_predictions.tsv and tweet_json.txt) was made and merge in single data file called (df_merge)
This is for the data to be cleaned, analyzed and properly visualized. 
Handle all the issues raised from the quality issue to the tidiness issues. Then used this following steps --- 
Defining the issue, writing codes to handle the issue, and then testing my codes by running them on my Jupiter notebook to check if it runs properly without errors.
The last step was storing my data, analyzing and visualization them.
Storing:  stored my initial file as (df_merge as twitter_archive_master.csv)
Analyzing: Ran this new stored file (twitter_archive_master) by checking the file using some of this codes (.head(), .info(), .describe()) .
Visualizing: Created some tables and used statistical analyzation like bar chat, pie chat to answer some of the questions.

