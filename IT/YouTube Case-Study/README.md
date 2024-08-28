# YouTube Case-Study

## 1. Sentiment Analysis

The goal is to understand the sentiment of the audience and identify the most frequently used negative and positive words.

**Findings:**

The sentiment analysis revealed the most commonly used positive words were best, awesome, and perfect, indicating a high level of satisfaction and approval. In contrast, the most frequently used negative words were worst, terrible, and boring, suggesting areas where improvements could be made.

                                                  Positive WordCloud
![Positive WordCloud](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/positive%20wordcloud.jpg)

                                                  Negative WordCloud
![Negative WordCloud](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/negative%20wordcloud.jpg)

**Tools and Techniques:**

* Programming Language: Python
* Libraries: Pandas, NumPy, Matplotlib, Seaborn, TextBlob, WordCloud, Emoji, Plotly

## 2. Emoji Analysis

The goal is to identify the most commonly used emojis.

**Findings:**

The emoji analysis revealed the following top 10 most frequently used emojis:

* 😂 (Laughing face)
* 😍 (Heart eyes)
* ❤ (Heart)
* 🔥 (Fire)
* 😭 (Crying face)
* 👏 (Clapping hands)
* 😘 (Kissing face)
* 👍 (Thumbs up)
* 💖 (Sparkling heart)
* 💕 (Heart with wings)

These emojis suggest that the audience is primarily expressing positive emotions such as joy, love, excitement, and approval. However, there is also evidence of negative emotions, such as sadness and frustration.

                                                  Top ten frequently used emojis

![Emojis](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/emoji.jpg)

## 3. Understanding Viewer Reactions for each video (sentiment counts)

The goal is to understand the distribution of sentiments (negative, neutral, positive) across various YouTube videos.

**Findings:**

The analysis revealed the following sentiment distribution for the YouTube videos:

| Video ID | nan | Negative | Neutral | Positive | Total Comments |
|---|---|---|---|---|---|
| JinobXWPk | 47 | 1 | 51 | 1 | 100 |
| -1fzGnFwz9M | 68 | 0 | 30 | 2 | 100 |
| -3AGlBYyLjo | 3 | 0 | 1 | 0 | 4 |
| ... | ... | ... | ... | ... | ... |
| zqE-ultsWt0 | 305 | 2 | 183 | 10 | 500 |
| zrOHeEA14kQ | 257 | 0 | 240 | 0 | 497 |
| zuKX0fPlo2Q | 2 | 0 | 0 | 0 | 2 |
| zuUQDdWNAPc | 95 | 0 | 101 | 4 | 200 |
| zyPIdeF4NFI | 246 | 0 | 132 | 22 | 400 |

**Explanation of nan Values:**

The "nan" values in the dataset indicate that the corresponding comment could not be classified as positive, negative, or neutral. This might be due to various reasons, such as:

* Ambiguous Content: The comment might contain mixed or unclear sentiments.
* Lack of Sentiment Words: The comment might not contain enough words or phrases that can be associated with positive or negative emotions.
* Different Language: The comments could be in different languages.

It's important to note that "nan" values are not null values. They represent a specific category in this analysis, indicating that the sentiment could not be determined.

## 4. Analyzing Comment Length and Sentiment

The goal is to determine if there is a correlation between the length of a comment and its sentiment.

**Findings:**

The analysis revealed a weak negative correlation between comment length and sentiment. This indicates that longer comments are slightly more likely to be negative than shorter comments. However, the correlation coefficient of -0.008709 suggests that the relationship is weak and not statistically significant.

                                                  Sentiment vs Comments Length

![sentiment vs comments len](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/sentiment%20vs%20comment%20length.jpg)

## 5. Analyzing Likes and Sentiment

The goal is to determine if there is a correlation between the polarity of a comment and the number of likes it gets.

**Findings:**

The analysis revealed a very weak negative correlation between comment polarity and likes. This indicates that comments with slightly negative sentiments tend to receive slightly more likes than those with positive or neutral sentiments. However, the correlation coefficient of -0.0007664447517908679 suggests that the relationship is extremely weak and not statistically significant.

                                                  Sentiment vs Likes

![sentiment vs likes](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/sentiment%20vs%20likes.jpg)

## 6. Analyzing Most Liked Category and Sentiment

The goal is to determine which category receives the most likes.

**Findings:**

The analysis revealed that **Music** is the most liked category of YouTube videos.

                                                  Most Liked Categories

![most liked category](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/most%20liked%20category.jpg)

## 7. Analyzing Audience Engagement

The goal is to determine which categories are most engaging and analyze the relationships between views, likes, and dislikes.

**Findings:**

**Most Engaging Categories:**

* **Most Liked:** Entertainment (90.3%)

                                                  Categories vs Likes Rate

![Categories vs Likes rates](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/category%20vs%20likes%20rates.jpg)

* **Most Disliked:** People & Blogs (73.11%)

                                                  Categories vs Dislikes Rate

![Categories vs Dislikes rates](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/category%20vs%20dislikes%20rates.jpg)

* **Most Comments:** Howto & Style (59.90%)

                                                  Categories vs Comments Rates

![Categories vs comments count rates](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/category%20vs%20comments%20count%20rates.jpg)

**Correlation Analysis:**

|  | Views | Likes | Dislikes |
|---|---|---|---|
| Views | 1.000000 | 0.779531 | 0.405428 |
| Likes | 0.779531 | 1.000000 | 0.451809 |
| Dislikes | 0.405428 | 0.451809 | 1.000000 |

![Heatmap](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/heat%20map%20for%20views%20likes%20and%20dislikes.jpg)

**Interpretation:**

* The strong positive correlation between views and likes indicates that videos with more views tend to receive more likes.
* The moderate positive correlation between views and dislikes suggests that popular videos (with more views) are also more likely to receive dislikes.
* The moderate positive correlation between likes and dislikes implies that videos that receive more likes are also more likely to receive dislikes.

                                                  Views vs Likes

![views vs likes](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/views%20vs%20likes.jpg)

## 8. Analyzing Trending Videos

The goal is to determine which channels produce the most trending videos.

**Findings:**

The analysis revealed that **The Late Show with Stephen Colbert** is one of the most trending channels on YouTube.

                                                  Trending Videos

![trending videos](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/trending%20videos.jpg)

## 9. Analyzing Title Words and Sentiment

The goal is to determine which words are frequently used.

**Most Common Words:**

The most common word in YouTube video titles is the hyphen (-). This suggests that hyphens are often used to separate words or create compound terms in video titles.

                                                  Most Common Words in Video Titles

![title common words](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/title%20word%20analysis%20with%20puctuation.jpg)

When the punctuations are removed, the word "de" becomes the most common word. This could imply a few things:

* **Language Preference:** The dataset might contain a significant number of videos in languages where "de" is a common word or prefix (e.g., Spanish, Dutch, German).
* **Topic Trends:** The word "de" might be frequently used in specific topics or niches that are popular on YouTube.
* **Title Formatting:** "De" could be used as part of a specific naming convention or style often employed in YouTube video titles.

                                                  Most Common Words in Video Titles without Punctuations

![title common words without punctuations](https://github.com/SagaChikhale/Data-Analysis/blob/master/IT/YouTube%20Case-Study/images/title%20word%20analysis%20without%20puctuation.jpg)
  
