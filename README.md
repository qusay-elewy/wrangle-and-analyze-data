# Wrangle and Analyze Data

In this project, I document my wrangling efforts in a Jupyter Notebook. I also showcase them through analyses and visualizations using Python (and its libraries). The dataset that I will be wrangling, analyzing, and visualizing here is the tweet archive of Twitter user [@dog_rates](https://twitter.com/dog_rates), also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog.

## Project Steps Overview
My tasks in this project are as follows:
* Step 1: Gathering data (from multiple sources)
* Step 2: Assessing data (both visually and programmatically)
* Step 3: Cleaning data
* Step 4: Storing data
* Step 5: Analyzing, and visualizing data
* Step 6: Reporting
    * My data wrangling efforts
    * My data analyses and visualizations

## The Data
In this project, I will work on the following three datasets:
### Enhanced Twitter Archive
The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. Of the 5000+ tweets, Udacity has filtered for tweets with ratings only (there are 2356). This archive is saved under this name: twitter_archive_enhanced.csv.
### Additional Data via the Twitter API
Twitter archives are vert basic, and a lot of information is missing in it, such as retweet count and favorite count. For this reason, Udacity has provided a json file called  tweet_json.txt, which contains Tweet's entire set of JSON data.

In this project, I have read this .txt file line by line into a pandas DataFrame with tweet ID, retweet count, and favorite count.
### Image Predictions File
Udacity ran every image in the WeRateDogs Twitter archive through a neural network that can classify breeds of dogs. The results: a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction. The data is saved in a file called image_predictions.tsv, which is hosted on Udacity's servers and should be downloaded programmatically using the Requests library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

## Project Files
* __wrangle_act.ipynb:__ contains the structure of this project. Here, I wrote my code for gathering, assessing, cleaning, analyzing, and visualizing data.
* __twitter_archive_enhanced.csv__: given, and added manually to the project.
* __tweet_json.txt:__ given, and added manually.
* __image_predictions.tsv:__ file downloaded programmatically.
* __wrangle_report.pdf:__ briefly describes my wrangling efforts. This was framed as an internal document.
* __act_report.pdf:__ communicates some of the insights and displays the visualization(s) I produced from my wrangled data. This was framed as an external document, like a blog post or magazine article, for example.
* __twitter_archive_master.csv:__ The output of my wrangelling effort (i.e., combined and clean data) has been saved in this file.

