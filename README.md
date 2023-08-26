# Fake News Classifier

Hey there, fellow data enthusiasts! Welcome to my Fake News Classifier repository. In this exciting project, I took on the challenge of developing a machine learning program to identify potentially fake news articles. Let me walk you through my journey.

## The Task
The main goal of this project was to create a classifier that could distinguish between reliable news articles and articles that might be fake. The competition evaluation metric was accuracy, a straightforward measure that treats false positives and false negatives equally.

## The Dataset
The dataset for this project was provided by the competition organizers.The link to the dataset is [here](https://www.kaggle.com/competitions/fake-news/data). The description of the dataset is as follows:

train.csv: A full training dataset with the following attributes:

- id: unique id for a news article
- title: the title of a news article
- author: author of the news article
- text: the text of the article; could be incomplete
- label: a label that marks the article as potentially unreliable
  - 1: unreliable
  - 0: reliable

test.csv: A testing training dataset with all the same attributes at train.csv without the label.

submit.csv: A sample submission that you can submit to the competition.

## My Approach
For this project, I decided to go with an LSTM (Long Short-Term Memory) model. LSTMs are super cool because they're capable of capturing long-range dependencies in sequences, which makes them a great fit for tasks involving text data like this one.

## Implementation
Here's how I went about it:

- **Dependencies:** I made sure to have TensorFlow installed (`pip install tensorflow`), as it's the backbone of my machine learning endeavors.

- **Cloning the Repo:** I cloned the project repository to get started: `git clone https://github.com/shro-2002/Fake_News_Detection.git`

- **Model Training:** I created and trained my LSTM model using the provided training data. This involved preparing the data, defining the architecture of the LSTM network, and compiling the model. I used the Adam optimizer and binary cross-entropy loss.

- **Predictions:** With my trained model, I generated predictions for the test dataset. These predictions were based on whether an article was likely fake or not.

- **Submission File:** The competition required a specific format for submission. I created a CSV file containing two columns: `id` and `label`. I used 0 to indicate a reliable article and 1 for articles that were potentially fake.

## Reflection
This project was an incredible learning experience. I got hands-on with LSTM models, learned about text data preprocessing, and gained insights into model evaluation using accuracy. I'm proud to say that I successfully tackled this competition and created a robust fake news classifier.

Feel free to explore my repository, and if you have any questions or suggestions, don't hesitate to get in touch. Happy coding! 🚀
