# SpamNet: Custom NN & Word2Vec for Spam Detection

This project demonstrates a custom approach to building and evaluating a two-layer neural network for spam detection. The implementation includes creating Word2Vec embeddings using logistic regression with negative sampling from scratch, emphasizing a deep understanding of both feature extraction and model training, evaluated through standard metrics.

## Objectives

### Dataset Preparation
- **Data Preprocessing:**  
  Clean and balance the spam dataset, including tokenization and noise removal.
- **Dataset Selection:**  
  Utilize the [Spam or Not Spam Dataset](https://www.kaggle.com/datasets/ozlerhakan/spam-or-not-spam-dataset?resource=download) from Kaggle for training and testing.

### Model Development
- **Custom Word2Vec:**  
  Build word embeddings using a logistic regression approach with negative sampling (embedding size = 10), implemented entirely from scratch.
- **Neural Network Construction:**  
  Design a two-layer feed-forward neural network with:
  - **Input:** 12 words per sample (each represented by a 10-dimensional embedding)
  - **Hidden Layer:** 2 nodes (each with 8 units)
  - **Output:** 1 node for binary classification

### Training and Evaluation
- **Model Training:**  
  Implement forward and backward propagation, and use stochastic gradient descent (SGD) for optimization.
- **Performance Metrics:**  
  Evaluate the model using accuracy, precision, recall, and F1 score.
- **Visualization:**  
  Generate a confusion matrix to visually assess model performance.

### Visualization and Analysis
- **Training Insights:**  
  Log key metrics such as loss and evaluation scores at each epoch.
- **Result Analysis:**  
  Use plots and the confusion matrix to analyze model convergence and performance trends.

## Training Log

During training, key metrics are logged per epoch. For example:

```plaintext
Epoch [1/50] | Train Loss: 0.875 | Val Loss: 0.912 | Accuracy: 82.5%
Epoch [2/50] | Train Loss: 0.823 | Val Loss: 0.876 | Accuracy: 83.7%
...
Epoch [50/50] | Train Loss: 0.412 | Val Loss: 0.445 | Accuracy: 91.2%
 ```
## Clone the Repository
```bash
git clone https://github.com/tallal02/SpamNet.git
cd SpamNet
