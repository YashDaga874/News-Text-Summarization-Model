

# News Summary using Seq2Seq LSTM Model

This repository contains code for building a text summarization model using Seq2Seq LSTM architecture. The model is trained on a dataset consisting of news articles collected from various sources, including Inshorts, Hindu, Indian Times, and Guardian, spanning from February to August 2017.

## Project Overview

Text summarization is a crucial task in natural language processing, aiming to condense long pieces of text into concise summaries while retaining the essential information. This project explores the implementation of a Seq2Seq LSTM model for this purpose.

### Features

- **Dataset**: The dataset comprises 4515 news articles with fields such as Author Name, Headlines, URL of Article, Short Text, and Complete Article.
- **Data Cleaning**: Extensive preprocessing including text cleaning, tokenization, and rare word analysis was performed to prepare the data for training.
- **Model Architecture**: The model utilizes an Encoder-Decoder architecture with LSTM units, incorporating attention mechanisms for improved summarization performance.
- **Training**: The model was trained on a subset of the data, focusing on articles with summaries containing up to 15 words and main texts with up to 100 words.
- **Evaluation**: Performance metrics such as loss function (sparse categorical cross-entropy) were monitored during training to assess model convergence and effectiveness.

## Setup

To run this project locally, ensure you have the following dependencies installed:

- Python 3
- TensorFlow/Keras
- NumPy
- Pandas
- Matplotlib
- spaCy

## Usage

1. **Data Preparation**: Ensure your dataset is in CSV format as described (`news_summary.csv` and `news_summary_more.csv`).
2. **Preprocessing**: Run the preprocessing scripts (`data_preprocessing.ipynb`) to clean and tokenize the text data.
3. **Model Training**: Execute the model training script (`seq2seq_model.ipynb`) to train the LSTM model.
4. **Evaluation**: Monitor training/validation loss to gauge model performance.
5. **Inference**: Implement inference scripts to generate summaries for new input texts using the trained model.

## Resources

For further reading and understanding of the concepts used in this project, refer to the following resources:

- [Comprehensive Guide to Text Summarization using Deep Learning](https://www.analyticsvidhya.com/blog/2019/06/comprehensive-guide-text-summarization-using-deep-learning-python/)
- [Introduction to Text Summarization with TextRank](https://www.analyticsvidhya.com/blog/2018/11/introduction-text-summarization-textrank-python/)
- [Building a Text Summarizer using Deep Learning](https://towardsdatascience.com/understand-text-summarization-and-create-your-own-summarizer-in-python-b26a9f09fc70)

## Acknowledgments

- Special thanks to the authors of Inshorts for providing the initial dataset and inspiration for this project.

## Contributing

Contributions to enhance the project and extend its functionalities are welcome. Please fork the repository, create a new branch, commit your changes, and open a pull request.

---

Feel free to adjust the sections, add more details, or include specific instructions based on your implementation and preferences. This template provides a structured approach to presenting your project on GitHub.
