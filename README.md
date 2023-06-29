# 'PBS Space Time' YouTube Channel Analysis
This project aims to analyze the data from 'PBS Space Time' YouTube channel. The dataset used in this analysis consists of video statistics such as the number of likes, views, comments, etc. This project is inspired by Thu Vu's guided project https://www.youtube.com/watch?v=D56_Cx36oGY&t=2s where she scrapes the data using youtube API, pre-processes the data, and performs Exploratory Data Analysis.

**Check out https://www.kaggle.com/code/snipss2/youtube-channel-analysis/edit/run/134154756 for Exploratory Data Analysis** 

Libraries used are Pandas, Numpy, Plotly, matplotlib, Seaborn, NLTK and WordCLoud.

# Data Collection
The data were collected using the YouTube Data API, which provides access to YouTube's features, including video search, video details, and comments. The following steps were taken to collect the data:
- Set up a project in the Google Cloud Console and enable the YouTube Data API.
- Obtained an API key to authenticate requests to the YouTube API.
- Used the YouTube Data API to search for videos from 'The Secrets of the Universe' channel and retrieve their video IDs and titles.
- Retrieved the comments for each video using the video IDs.
  
# Data Preprocessing
Before performing any analysis, the collected data underwent preprocessing to clean and transform it into a suitable format. The following preprocessing steps were performed:
- Removed NaN values
- Changed the Data Types of some features
- Removed irrelevant columns
  
# Exploratory Data Analysis (EDA)
The EDA phase involved gaining insights into the 'PBS Space Time' YouTube channel data. The following analyses and visualizations were performed:
- Analyzed which videos were most and least viewed
- Amount of videos uploaded in days
- Heatmap to find a correlation between numerical columns
- Which videos have the most comment counts
- Number of tags associated with videos
- Determined the relationship between like counts and comment counts vs view counts
  
# WordCLoud
- Used NLTK and WOrdCLoud to build a wordcloud using processed titles of the videos. Processed titles consists of video titles without stop words.
- USed PIL for masking an image on a wordcloud.
  
# Project limitation:
- Sentiment Analysis could not be performed because random comments from all the videos were extracted which might not have been an accurate representation of all comments
- There are many other factors that haven't been taken into analysis, including the marketing strategy of the creators and many random effects that would affect how successful a video is
- 
# References/ Resources used:
[1] Youtube API. Available at https://developers.google.com/youtube/v3

[2] Converting video durations to the time function. https://stackoverflow.com/questions/15596753/how-do-i-get-video-durations-with-youtube-api-version-3

Video Category Distribution: Examined the distribution of video categories to understand the content focus of the channel. View and Like Analysis: Investigated seasonal trends in the number of views and likes to identify any patterns or variations.
