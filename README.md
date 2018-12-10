# data512-a6

This repository is part of the final project submission for DATA 512 course by Vamsy Atluri. Materials in this repository are released under the MIT License.

## Abstract

Nowadays, the industry and media claim that gender diversity is improving and more and more women are playing major roles than ever. At the same time, companies like Google, Facebook, Amazon etc. have started to enforce gender equality requirements trying to make the workplace more diverse. They have also been releasing yearly diversity reports to show the increase in diversity.

The aim of this project is to analyze IMDB's actor and movie datasets for gender statistics in terms of number of actors and actresses potrayed on the screen every year, visualize the statistics obtained for the time period over which data is available and then compare the results to the diversity percentages released by tech companies Facebook, Amazon, Apple, Google and Microsoft. Off the bat, the feeling is that both were male dominated industries for several decades and might still be. But has there been a change in this percentage over the years?


## Data

The primary sources of data used in this project are from IMDB, which are hosted [here](https://datasets.imdbws.com/). The data is updated periodically and can be downloaded directly from this link.

A desciption of the datasets and the various fields are given [here](https://www.imdb.com/interfaces/). 

Each dataset is contained in a gzipped, tab-separated-values (TSV) formatted file in the UTF-8 character set. 

The first line in each file contains headers that describe what is in each column. A ‘\\N’ is used to denote that a particular field is missing for that title/name --- ([reference](https://www.imdb.com/interfaces/)).

The data for diversity statistics for companies were taken from their public posts on their sites at [Facebook](https://newsroom.fb.com/news/2018/07/diversity-report/), [Apple](https://www.apple.com/diversity/), [Google](https://diversity.google/annual-report/), [Microsoft](https://www.microsoft.com/en-us/diversity/inside-microsoft/default.aspx) and [Amazon](https://www.amazon.com/b?ie=UTF8&node=10080092011)

## Reproducibility

### Tools and Software Required

A computer with python2 or python3 installed is required to reproduce this analysis. In addition, the libraries [pandas](https://pandas.pydata.org/), [numpy](http://www.numpy.org/) and [matplotlib](https://matplotlib.org/) are required. They can be installed using [pip]. For e.g. to install pandas, run  ```pip install pandas``` from your CLI.

### Getting the data

To get the entire dataset, please download the data from the IMDB [website](https://datasets.imdbws.com/). This will ensure you have the latest data available. You can either change the path for the source files in the notebook or ensure the files are in the same folder as the notebook and you should be good to go.

You can also use the sample files in the data folder of this repository. This is a sample subset of the original data which is too big to host on Github.

### Doing the analysis

Simply run the 'DATA512_A6_Report.ipynb' notebook. First, download the notebook and navigate to that folder in the CLI. Then run ```jupyter notebook``` in the CLI and select this notebook in the window that opens. If jupyter notebook is not installed please follow instructions [here](http://jupyter.org/install).

The analysis is very straightforward and well documented so you do not need to be a data scientist or very familiar with code to follow!

## Findings

Detailed images and analysis of the data can be found in the DATA512_A6_Report.ipynb notebook. To summarize the findings:

Finding 1 : As expected, we see that the number of actors in the industry has always been higher than the number of actresses. The gap between the two looks to be highest just before 1960. While the situation looked to be improving for a while, the gap appears to have suddenly blown up in the last decade or so -- with a highly disproportionate number of actors dominating the scene as compared to actresses.

![Diversity over the years](https://github.com/whamsy/data512-a6/blob/master/images/1.png)

Finding 2: Comparing the percentages gives a much cleare picture of how gender diversity has played out in the movies. The lowest percentage of actresses in the industry appears to be just before 1960 with a noticeable increase in the years following. There also appears to be a spike post 1990.

![Diversity over the years](https://github.com/whamsy/data512-a6/blob/master/images/2.png)

Finding 3: By comparing statistics for 2017 alone, gender diversity in movies while not very high was still highly comparable to that of Amazon while significantly better than Facebook, Apple, Microsoft and Google. This was a little suprising for me because I would have expected movies to do a little worse than the tech firms, not better than most of them.

![Movies vs Global Tech](https://github.com/whamsy/data512-a6/blob/master/images/3.png)

Finding 4 - If we compare gender diversity in movies in terms of actors/actresses to only tech force diversity in the tech industry then the movies outrank them all. Movies have around a 60/40 split leaning more towards actors, but the closest any tech firm comes is Apple with a mere 23% of their tech force comprised of females.

![Movies vs Tech Workers only](https://github.com/whamsy/data512-a6/blob/master/images/5.png)

In conclusion, It's tough to compare the two sectors, specially without more information of people behind the camera. Actors/actresses are a very small percentage of the movie industry and might not be representative of the industry at large. But if we consider only actors/actresses, there seems to be more diversity in the movies than tech companies specially when comparing only the tech working force.

## Licensing

The data is made available by IMDB for personal and non-commercial use, as stated on this [page](https://www.imdb.com/interfaces/).

Local copies of the data can also be stored.  

But IMDB prohibits data mining, robots, screen scraping, or similar data gathering and extraction tools. None of these techniques have been used to access the data, which has been downloaded from IMDB's public dataset [link](https://datasets.imdbws.com/).

More information about non-commerical licensing is given on the IMDB [website](https://help.imdb.com/article/imdb/general-information/can-i-use-imdb-data-in-my-software/G5JTRESSHJBBHTGX?pf_rd_m=A2FGELUUNOQJNL&pf_rd_p=3aefe545-f8d3-4562-976a-e5eb47d1bb18&pf_rd_r=BMZ4YZDQZXG5J9Y3H7RJ&pf_rd_s=center-1&pf_rd_t=60601&pf_rd_i=interfaces&ref_=fea_mn_lk1#).

### Course Wiki

Thanks to Jonathan and Os for a wonderful quarter! The wiki for this course can be found [here](https://wiki.communitydata.cc/Human_Centered_Data_Science_(Fall_2018))
