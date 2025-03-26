+++
author = "Xingran Wang"
title = "Data Wrangle and Analyze for Twitter DataSet"
date = "2023-03-26"
description = " "
summary = "The purpose of thihs project is to Wrangle Twitter dataset for a popular account to create interesting and trustworthy analyses and visualizations. To better understand the data analysis process and the coding techniques for data analysis with python. [Read More](https://ariawxr.github.io/post/test/)"

tags = [
    "python",
    "Numpy",
    "tweepy"
]
categories = [
    "data analysis",
    "data visualization",
]
series = ["Data Analysis"]
aliases = ["migrate-from-jekyl"]
+++

The dataset is the tweet archive of Twitter user @dog_rates. It is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. 

The purpose of thihs project is to Wrangle WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations. By completing this project, i got a better understanding of the data analysis process and the coding techniques for data analysis. At the end, i also learned to apply python library to cxreate data visualizations.

## Introduction of Dataset

- **twitter_archive_enhanced.csv** ( download manually )

- **image_predictions.tsv**: The tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file (image_predictions.tsv) is hosted on Udacity's servers and should be downloaded programmatically using the Requests library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

- **tweet_json.txt**: Each tweet's retweet count and favorite ("like") count at minimum. Using the tweet IDs in the WeRateDogs Twitter archive, query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of JSON data in a file called tweet_json.txt file. Each tweet's JSON data should be written to its own line. Then read this .txt file line by line into a pandas DataFrame with (at minimum) tweet ID, retweet count, and favorite count. 

Above 3 datasets can also be found in my [Github](https://github.com/AriaWXR/ariawxr.github.io/tree/main/twitter%20project).

## Flowchart for Project

Below is the flowchart for the project, for this project, the data cleaning is conducted by 2 main parts. for each part, i summarized the issues i met in the dataset and solved them one by one. Then after exploring the potential questions, i made my conclusions for the insights through the data.

{{< figure
  src=/images/project1/flowchart1.png
  alt=" "
  caption=" "
  loading=lazy
  width="2000px"
>}}

## Conclusions

_**Conclusion 1:**_

According to my plot, most of the retweet are below 40000 and most of the favorite count are below 80000. No matter what stage it is, there seems to be more favorite counts than retweet counts, which is understandable. An interesting finding is that doggo, puppo and pupper seem to gain more retweets and favorite counts. Dog stage is very likely a factor affecting the retweet counts and favorite counts.

<img src="/images/project1/chart1.png" alt="imsf" class="medium-zoom-image" width="1800px">

_**Conclusion 2:**_

According to the plot, we can see there are two activity peaks 0-3 and 16-17. Users like to post tweets either at the time before off work or late night(even 3 am belongs to early morning but It is more likely they stay late until 3 am rather than they get up at 3 am to post tweets).

It is shown that tweets posted at evening time or late night gains more retweets and favorites. It is generally consistent with the two activity peaks. More users are active at the peorids, which generate more retweets and favorite counts.

<img src="/images/project1/chart2.png" alt="imsf" class="medium-zoom-image" width="1800px">

<img src="/images/project1/chart3.png" alt="imsf" class="medium-zoom-image" width="1800px">

_**Conclusion 3:**_

There is a large number of unidentifiable breed. I tried to investigate the reasons. One reason is that the picture has nothing to do with dogs. They are totally unrelated tweets. The top 3 popular tweeted breeds are golden retriever , labrador retriever and pembroke.

<img src="/images/project1/chart4.png" alt="imsf" class="medium-zoom-image" width="1800px">

### Used Library in Python

- pandas
- NumPy
- requests
- tweepy
- json

### Useful links

Code:

- https://github.com/AriaWXR/ariawxr.github.io/blob/main/twitter%20project/wrangle_act.ipynb

Dataset:

- https://github.com/AriaWXR/ariawxr.github.io/blob/main/twitter%20project/image-predictions.tsv
- https://github.com/AriaWXR/ariawxr.github.io/blob/main/twitter%20project/tweet-json.txt
- https://github.com/AriaWXR/ariawxr.github.io/blob/main/twitter%20project/twitter-archive-enhanced.csv 
```<img src="/images/landscape.jpg" alt="imsf" class="medium-zoom-image" width="100px">
```
```[link name](https://github.com)
```
