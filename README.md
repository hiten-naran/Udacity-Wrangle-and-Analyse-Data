# Udacity Wrangle and Analyse Data

This was the 3rd Udacity Data analyst project which I worked on. 

## Project Overview

Real-world data rarely comes clean. Using Python and its libraries, I gathered data from a variety of sources and in a variety of formats, assessed its quality and tidiness, then cleaned it. This process is called data wrangling.

The dataset wrangled was the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage.

WeRateDogs downloaded their Twitter archive and sent it to Udacity via email exclusively for you to use in this project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017. More on this soon.

## The Datasets used for analysis

### Enhanced Twitter Archive

The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, which was used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced." Of the 5000+ tweets, twitter with ratings only have been filtered (there are 2356).

### Additional Data via the Twitter API

Back to the basic-ness of Twitter archives: retweet count and favorite count are two of the notable column omissions. This additional data was gathered from Twitter's API.

### Image Predictions File

Udacity ran every image in the WeRateDogs Twitter archive through a neural network that can classify breeds of dogs. The results show a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images).

## Key files which I worked on and with to generate output

### Assessing and cleaning data

I conducted by wrangling, analysis and visualisation efforts across the following Jupyter Notebook file:

 - wrangle_act.ipynb
 
The following files were used to conduct my cleaning and wrangling efforts:

 - twitter_archive_enhanced.csv
 - image_predictions.tsv (this was downloaded programmatically from Udacity server's using the Request libaray and the following file https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv)
 - tweet_json.txt (this is file which stores data extracted from Twitter's API using the Tweepy library)

I stored the cleaned DateFrame into the following csv:

- twitter_archive_master.csv

### Reporting

I wrote up a written report to describe my wrangling efforts across the following files:

 - wrangle_report.pdf
 - wrangle_report.html

I wrote up a written report to communicate the insights and visualisations producted from wrangled data across the following files:

 - act_report.pdf
 - act_report.html



