
![Banner](wsb.png)
# r/wallstreetbets

## Motivation:
The main goal of this project was to perform knowledge discovery from real-world complex data. With this approach, it is necessary to perform a proper acquisition of data from various sources, to process them into an appropriate representation, to evaluate the quality of the data itself, to assess the validity of the features, to look for correlations between them, to discover useful and potentially interesting patterns, and then possibly to construct a classification model. It is also necessary to interpret and evaluate the induced knowledge. 

## Data context:
r/wallstreetbets, also known as WallStreetBets or WSB, is a subreddit where participants discuss stock and option trading. It has become notable for its colorful and profane jargon, aggressive trading strategies, harassment and for playing a major role in the GameStop (GME) short squeeze that caused losses for some US firms and short sellers in a few days in early 2021. Source: [kaggle.com](https://www.kaggle.com/datasets/gpreda/reddit-wallstreetsbets-posts)

## Tasks
The task was to create a model that predicts the popularity of of user posts depending on their content, time of publication and GME stock price at a given time. The analysis should answer to questions such as: Is there a recipe for a popular post? Is that possible to predict the long-term success of a post based on the progression of the the post discussion during the first hours after publication? Is is there a correlation between GME stock price and WSB users activity?

## Solution
The analysis was organized into following sections:
### 1. Non visual features:
- Exploratory data analysis
- NLP
- Sentiment analysis
- Other atributes like stock prices, date attributes, emoji etc.

### 2. Visual features:
- Text recognition using [keras_ocr](https://github.com/faustomorales/keras-ocr)
- Visual object recognition using [YOLOv5](https://github.com/ultralytics/yolov5)

### 3. Feature importance:
- Evaluation
- Correlations and other analyses
- Selection

### 4. Post popularity prediction:
- Preliminary algorithms test (autoML mode on) 
- Two algorithms chosen (CatBoost, DecisionTree)
- Knowledge for users - what to do in order to create a popular post

### 5. Time series data
- Comments retrieval
- Time series preparation

### 6. Discussion progression forecasting:
- Usage of time series created in previous step
- Assessment of the impact of comments from the first hour / two / five hours on the post popularity prediction