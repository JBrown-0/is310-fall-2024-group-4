The original document where we documented our work can be found [here](https://docs.google.com/document/d/1jiZu7202nsj72C1fidfOaHzQAlwRsdrb271cNmbg2gI/edit?tab=t.0)
# **Methods + Data Selection**



## 1. **Three Computational Methods**

*  Statistical Analysis (Regression Models) 
    
*  Sentiment Analysis: identify and categorize opinions within a large collection of data, usually text. So, Tweets on Twitter would be perfect

*  Topic modeling: Used to identify "topics," within large collections of text. Groups words that frequently appear together into topics, and reveals the main subjects discussed in a textual dataset. For example: Latent Dirichlet Allocation (LDA), which categorizes documents by assigning each a probability distribution across multiple topics.

## 2. **Two Cultural Data Types**

### Twitter posts and Instagram posts

Explore tweets/posts related to players, injuries, games, events, signings etc. Posts and comments reflect how people are talking about what’s going on in the NBA, such as opinions and reactions to news or events. Analyzing this can reveal common themes, slang, expressions of fandom, and sentiments about teams or players. Gather data on engagement: views, captions, comments, likes, shares, follower counts, etc to gauge the cultural impact of tweets

Additionally, we can  use topic modeling to split posts into “topics” by gathering posts from NBA team accounts to analyze the text and images associated with each post. Also, we can gather the engagement per post to understand how followers engage with certain topics. We then can associate overall engagement with each topic that the model creates and visualize the distribution of topics among an NBA team’s Instagram posts


# **Scholarships**

* (Alan) [Analysis of Instagram Post Engagement through Topic Modeling](https://github.com/Abdul-AA/Instagram-post-analysis) 
* (Justin) Instagram Alt Texts [https://accessibility.huit.harvard.edu/describe-content-images](https://accessibility.huit.harvard.edu/describe-content-images), [https://help.instagram.com/503708446705527](https://help.instagram.com/503708446705527)
* (Haydn) [https://www.pnas.org/doi/abs/10.1073/pnas.1719792115](https://www.pnas.org/doi/abs/10.1073/pnas.1719792115)
* (Alex) Twitter Topic Modeling [https://link.springer.com/chapter/10.1007/978-3-031-18840-4_15](https://link.springer.com/chapter/10.1007/978-3-031-18840-4_15)(access through UIUC library), [https://jmausolf.github.io/code/Topic_Models_for_Text/](https://jmausolf.github.io/code/Topic_Models_for_Text/)
* (Ahmad) [Leveraging AI for Fan Sentiment Analysis | DSI | Vanderbilt University](https://www.vanderbilt.edu/datascience/2024/08/13/nashville-sc-leveraging-ai-for-fan-sentiment-analysis/) 


# **Scholarship Summaries**

## **Topic Modeling for Instagram Posts (Alan)**

[Analysis of Instagram Post Engagement through Topic Modeling](https://github.com/Abdul-AA/Instagram-post-analysis) 

I found a Github repo that uses Topic modeling to understand how images in Instagram posts and the engagement on them create themes. Takes advantage of Google Vision to identify what the images in an Instagram post are conveying.


1.  Analysis of Instagram Post Engagement through Topic Modeling.



* Published by Abdulrahman Aroworamimo via a Jupyter Notebook shared on Github on May 2, 2024.

2. Methods



* Computational Method:s
    * Image Labeling: Images from Instagram posts were labeled using the Google Vision API to identify descriptive keywords.
    * Topic Modeling: Latent Dirichlet Allocation (LDA) was used to group captions and image labels into eight distinct topics. Each image was then assigned a probabilistic distribution across these topics.
    * Engagement Analysis: Post engagement was measured based on the number of comments, categorizing posts into high and low-engagement groups to compare topic relevance.
* The data of Instagram images and captions were transformed into text-only labels that were generated by Google Vision. Then, these labels were grouped into themes/topics, which were then analyzed for patterns in user engagement.

3. Argument



* “The goal is to identify which topics are associated with higher engagement, defined as the number of comments. This information can guide content strategy to increase engagement on the platform.”
* When looking in the notebook for the results I found that certain content topics on Instagram are associated with higher engagement levels. Posts related to sports, formal events, and outdoor leisure tend to perform better in terms of comments. Topics like casual wear and digital branding show lower engagement, suggesting potential areas for content reevaluation.
* The LDA package included commands that would sort these images into common themes/topics by weighing the relationship between each topic and comments

4. Sample Code



* It uses a Python notebook for all the work. Scanning and identifying what’s going on in the images is done with Google Vision.  LDA is also used for topic modeling the images’ text descriptions. And packages like pandas is used for data cleaning, analyzing, and visualization.
* The dataset is 1522 images across a sample of 296 Instagram posts. The publisher did not specify whether the posts came from the same account or not.

5. What was interesting



* The Google Vision Python package looks super interesting and seems to do a good job of identifying what’s in a digital image. I do wonder what the runtimes of processing images would look like, as AI tends to be resource-intensive when working.
* This work would fall under Digital Humanities as it’s using a computational method of analyzing digital social media posts using algorithms to find patterns in their topics to study cultural topics from digital media..

6. Usefulness: This study demonstrates how post(s) content can be quantitatively linked to content themes, which is directly applicable to our NBA social media project. What we can gather from topic modeling can reveal common themes on NBA teams’ Twitter and Instagram to understand what NBA teams want their social media presence to look like


## **Instagram Alt Texts (Justin)**

Instagram Alt Texts [https://accessibility.huit.harvard.edu/describe-content-images](https://accessibility.huit.harvard.edu/describe-content-images), [https://help.instagram.com/503708446705527](https://help.instagram.com/503708446705527)

1. I reviewed the article titled Through the Eyes of Instagram: Analyzing Image Content utilizing Meta’s Automatic Alt-Text, authored by João Francisco Hecksher Olivetti and Philipe de Freitas Melo. It was published in 2023 and is based out of Universidade Federal de Viçosa in Brazil.
2. This research examines the use of Meta’s Automatic Alt-Text (AAT) feature, which generates AI-driven descriptions for images on Instagram. AAT translates visual elements in the image into text descriptions, allowing researchers to study the content without the influence of captions. This approach uses computer vision to interpret images and creates a standardized form of data for analysis.
3. Olivetti and Melo argue that Meta’s AAT provides a way to look at Instagram images through an objective lens, offering insights into how visual content is categorized and perceived by an AI system. By analyzing these alt-text descriptions, the authors explore how visual content is shared and how it can be grouped into themes that could inform marketing, social behavior, or content strategies.
4. While the alt-text algorithm itself is proprietary to Meta, the article outlines how to scrape Instagram posts to collect alt-text data for research purposes. The authors provide their methodology for using AAT descriptions, but the actual source code from Meta isn't publicly shared.
5. I found it particularly interesting that AAT allows for a standardized approach to understanding image content without the ambiguity of human-created captions. It also has potential in Digital Humanities and Computational Social Sciences, fields that benefit from computational methods to analyze large datasets. This is especially useful for studying visual culture on platforms like Instagram.
6. This research could be extremely useful for analyzing Instagram content in a way that removes the subjectivity of captions. By focusing on alt-text descriptions, we could gain a clearer understanding of how audiences engage with visual elements in sports content, especially when comparing different types of images or themes.


![screensshot1](https://github.com/CultureAsData-UIUC/is310-fall-2024-group-4/blob/main/Computing%20Cultural%20Data/Screenshot%202024-11-12%20152209.png?raw=true)

![screenshot2](https://github.com/CultureAsData-UIUC/is310-fall-2024-group-4/blob/main/Computing%20Cultural%20Data/Screenshot%202024-11-12%20151824.png)


## **Measuring Discursive Influence Summary (Haydn)**

[https://www.pnas.org/doi/abs/10.1073/pnas.1719792115](https://www.pnas.org/doi/abs/10.1073/pnas.1719792115)

1. A. Gerow, Y. Hu, J. Boyd-Graber, D.M. Blei, J.A. Evans, Measuring discursive influence across scholarship, *Proc. Natl. Acad. Sci. U.S.A.*

    115 (13) 3308-3313, [https://doi.org/10.1073/pnas.1719792115](https://doi.org/10.1073/pnas.1719792115) (2018)

2. Citations are the data being used for the analysis. It is a dynamic topic model. Analysis of citations alongside discursive influence is used and it. I’m not entirely sure how the source code works, there are many different languages being used, including programming languages that I have not heard of. The team mentions that they even incorporate Nobel Prize data and that it boosts influence in accrediting citations to authors.
3. The team said that the analysis reveals that citations have a bias of crediting authors that persist in their fields over large periods of time, and they discount credit for works that are influential over many different subtopics. 
4. They perform in-depth analyses on collections of physics research (500,000 abstracts; 102 years) and scholarship generally (JSTOR repository: 2 million full-text articles; 130 years). The overview describes the preparation and analysis of a dataset containing 509,007 abstracts from the American Physical Society (APS), spanning from 1913 to 2015. Each abstract is tagged with metadata, including article type, journal, authors, and affiliations. To improve metadata quality, only documents with authors appearing in at least two documents and affiliations appearing at least three times were kept. This filtering left 74,459 variables across 251,382 documents from 1918 to 2015.
5. I would consider this analysis to be within the field of Digital Humanities due to the nature of the data. Accreditation to authors and awards seem like an interdisciplinary element of social culture. Authors are part of the ecosystem that is human culture & digital humanities. It’s also in human ethical and legal approaches to credit authors for their work, which definitely feels like a digital humanities problem to me.
6. This scholarship would be useful in that it provides an example of one of the methods that we could use. Though at this point, I think we’ve decided that we like topic modeling. However, this analysis still serves as an example and perspective of the different types of methods that we could’ve used. It may or may not sway us in future endeavors. Though, if we decided to use this form of analysis, this scholarship would be very useful to us in that it would guide us to perform our own analysis.

## **Twitter Topic Modeling Summary (Alex)**

[Twitter Topic modeling](https://link.springer.com/chapter/10.1007/978-3-031-18840-4_15)

1. The first study linked relates to how Athletes’ performances significantly shift when Twitter users @ the athlete before games, done by Otto von Guericke University, Magdeburg, Germany in 2022. The authors listed are Frank Dreyer, Jannik Greif, Kolja Gu ̈nther, Myra Spiliopoulou, and Uli Niemann. The title of the paper is *Data-Driven Prediction of Athletes’ Performance based on their Social Media Presence*. 
2. The idea of the study is to look at athletes' performances, and how they change when they get more or less Twitter @’s before games. They found there are significant changes in players' stats based on this variable. The study does not go into the technical methods of how they monitored this, but I have found another source to go into how it might’ve been possible. 
3. The second link is to a short GitHub tutorial on how to set up a topic modeling system in Python for text and Twitter by Joshua Gary Mausolf, an experienced Data Science employee who worked for Google and Meta. 
4. The model is complicated, using a few different python libraries like Sklearn. The basics of it is it groups topics from large datasets into specific groups that can be easily extracted. 
5. I found the most interesting part of the study to be how athletes actually are affected by social media. Having a statistical change in performance is something I wouldn’t expect, but makes sense. The method for collecting the data is also interesting, as although the script seems simple enough the packages are doing a lot of heavy lifting. I would say this is related to computational Social Science, because it analyzes how players interact with social media, specifically how they perform based on interactions. 
6. This article and code is relevant to the project because it is somewhat similar to what we want to do. Using topic modeling to analyze Twitter data specifically relating to sports tweets could be transferred to grouping NBA player tweet topics relating to performance, or something about how much or what NBA players tweet during the season and if it affects their performance on the court. 


## **Leveraging AI for Fan Sentiment Analysis(Ahmad)**

[Leveraging AI for Fan Sentiment Analysis | DSI | Vanderbilt University](https://www.vanderbilt.edu/datascience/2024/08/13/nashville-sc-leveraging-ai-for-fan-sentiment-analysis/) 

1. The author is Miguel Nunez, published on 8/13/2024. The Publication Venue is Vanderbilt University
2. Natural Language Processing and AI analysis were both techniques used to evaluate discussions about team performance, pricing, and more. This data was used for developing strategies that are targeted towards improving fan experience and engagement.
3. This study argues that AI sentiment analysis can give insight to sports organizations on fan engagement and ideas, which would in turn let them provide a better experience for the fans. The core of the study is how Nashville SC can boost fan engagement and satisfaction by understanding fan sentiment. Aspect Based Sentiment Analysis (ABSA) alongside Generative AI is used to support this argument. They would look at social media to see fan discussions about teams, players, stadiums, pricing, and much more. This allows them to see both negatives and positives. Natural Language Processing (NLP) tools were used to extract this information from sites like Reddit. Data Visualization techniques were also used in this study like histograms and tables to showcase these findings. 
4. The data that is available showcased categories that included points on team performance, coaching and management, stadium atmosphere, stadium amenities, pricing, media coverage, and miscellaneous. It included an average sentiment score for teams NSC, Predators, and Titans, the score was positive for NSC and Predators which indicates that the fans were happy with those teams' performances. The same measurements were used for the other categories and a conclusion was made from these data points. 
5. The thing I found most interesting from this research is one of the data points on pricing, fans from all three teams seemed to not like the pricing and it makes me wonder if the sports organizers took this into consideration going forward. I think research would be categorized as Computational Social Sciences because it uses methods such as NLP and ABSA to analyze large amounts of data and it gives insight into human behavior. 
6. This scholarship actually gives us insight into different methods that can be used for our own datasets and projects. Seeing how effective their methods were can give us inspiration going forward with techniques like NLP and ABSA. 


# **Our Selected methods**

*	Our group decided that we like topic modeling, and we will be using it going forward with our semester-long project. The example that we found for this type of computational method was made by a GitHub user named Abdul-AA. He analyzes Instagram posts to cover specific categories and the weights in which these categories garner engagement and following on the platform. In his conclusion, he determined that posts related to sports were one of the highest and most effective ways to increase audience engagement. We feel that it makes sense to use this approach due to the thoroughness and the overlap in our project as related to what Abdul created. He’s provided a great example to learn from and conceptually use for our project.
