# document-classification-cnn

- Type of problem: Multi-class Classification (Text)
- Objective: Predict which category does the given article belong to.
- Performance Metric: Improve the Accuracy Score.
- Solution:
1. Preprocessed and Extracted Mail IDs, Subjects, Content,and Categories from all ~19K text
files. Extensively used Regex and NLTK for text preprocessing tasks.
2. Transformed Texts to Sequences using Keras and performed analysis on sequence lengths to
provide appropriate Padding.
3. Created Word Embedding Matrix of unique words in our data using Glove to be later used as
weights in Neural Network.
4. Performed analysis on Class Distribution and computed Class Weights to be later used in
Neural Network.
5. Built a Convolutional Neural Network (CNN) using a combination of Embedding, Conv1d, Max
Pooling, Flatten, Dropout and Dense layers and implemented necessary callbacks.
6. Achieved an Accuracy Score of 0.81.
