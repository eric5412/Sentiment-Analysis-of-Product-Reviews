Sentiment Analysis of Product Reviews
================
## Introduction:
The scope of this project was to analyze Amazon Alexa product data to gain insights from reviews provided by customers. The analysis was done using Python.

* **Data Source:** Amazon Alexa Reviews dataset on [Kaggle](https://www.kaggle.com/datasets/sid321axn/amazon-alexa-reviews/#).

The first goal was to analyze the data to discover what was the most frequent rating, what was the overall customer sentiment,
and which product variations had the most reviews and the least reviews.

The second goal was to use Natural Language Processing to analyze the sentiment of the reviews,
to discover what the customers liked from the products, and to learn about what the customers
may have wanted improvements on. Analyzing customer sentiment is important,
because it allows a company to build upon business strategies and improve the experience of 
their customers.

<br>

## Data Analysis:

![A bar chart of rating distribution](/images/1.png)

Most of the product reviews had a rating of 5 stars. This suggests that the overall customer sentiment was positive.

<br><br>

![A pie chart of rating distribution](/images/2.png)

More than half of the reviews had 5 star ratings.

<br><br>

![A bar chart of feedback distribution](/images/3.png)

The overall sentiment of the reviews was positive.
* **90.92%** of the reviews were labeled as positive ((2,214 / 2,435) x 100 = 90.92%).<br>

* **9.08%** of the reviews were labeled as negative ((221 / 2,435) x 100 = 9.08%).<br><br>

<br>

![A bar chart of product variation distribution](/images/4.png)

There was a significant difference in the number of reviews between the most frequently reviewed product variation and the least frequently reviewed product variation.

<br>

## Natural Language Processing:

Upon inspecting the product reviews, some of the text included punctuation marks and some text included emojis. The text of the reviews was first preprocessed to remove any punctuation marks, to make the text lowercase, to remove emojis, and to remove stop words. Stop words are common words that do not contribute to the sentiment of the review.

<br>

A word cloud was created for the reviews that had a rating of 4 stars or 5 stars to gain insights into what words were frequently used in positive reviews.

![A word cloud of frequently used words in positive reviews](/images/5.png)

<br>

Positive reviews that contained the word "love" were examined:

![Some positive reviews](/images/5a.png)

<br>

Positive reviews that contained the word "use" were examined:

![Some positive reviews](/images/5b.png)

<br>

Positive reviews that contained the word "great" were examined:

![Some positive reviews](/images/5c.png)

<br>

**Insights from Positive Reviews:**
* Love the sound.
* Easy to use.
* Great sound quality.

<br><br>

A word cloud was created for the reviews that had a rating of 1 star or 2 stars to gain insights into what words were frequently used in negative reviews.

![A word cloud of frequently used words in negative reviews](/images/6.png)

<br>

Negative reviews that contained the word "work" were examined:

![Some negative reviews](/images/6a.png)

<br>

Negative reviews that contained the word "time" were examined:

![Some negative reviews](/images/6b.png)

<br>

Negative reviews that contained the word "disappointed" were examined:

![Some negative reviews](/images/6c.png)

<br>

**Insights from Negative Reviews:**
* Did not continue to work.
* Not working after charging more than one time.
* Product did not hear requests.

<br><br>

The sentiment of each review was then analyzed.
These are the first rows of the resulting data frame:

![Customer sentiment](/images/7.png)

The values in the sentiment column range from -1 (most negative) to 1 (most positive) and represent the overall sentiment of each product review. A value of 0 indicates a neutral sentiment.

<br><br>

Summary statistics were then calculated for the sentiment column.

![Customer sentiment statistics](/images/8.png)

The lowest sentiment value was -0.9839 and the highest sentiment value was 0.9946. The mean and the median values of the sentiment column were greater than 0.50, indicating that the overall sentiment of the reviews was positive.

<br>

## Findings:
* The most frequent rating for the product reviews was 5 stars.<br><br>
* The overall customer sentiment was positive, 90.92% of the reviews were labeled as 
positive and 9.08% of the reviews were labeled as negative.<br><br>
* The product variation that had the most reviews was Configuration: Fire TV Stick and the 
product variation that had the least reviews was Walnut Finish.<br><br>
* Customers commented that they liked the sound quality, but some reviews mentioned that the 
product did not continue to work.<br><br>
* The sentiment analysis indicated that the reviews were mainly positive about the products.<br><br>

**Please click [here](https://github.com/eric5412/Sentiment-Analysis-of-Product-Reviews/blob/main/Sentiment%20Analysis%20of%20Product%20Reviews.ipynb) for the entire project.**

<br><br>
<br><br>
