# Document Classification CNN

- Domain: Education
- Type of problem: Multi-class Classification (Text)
- Objective: Given an article, predict which category does it belong to.
- Performance Metric: Improve the Accuracy Score.
- Solution:
1. Preprocessed and Extracted Mail IDs, Subjects, Content,and Labels from all ~19K text files. Extensively used Regex and NLTK for text preprocessing tasks.
2. Transformed Texts to Sequences using Keras and performed analysis on sequence lengths to provide appropriate Padding to make all sequences of same length.
3. Created Word Embedding Matrix of unique words in our data using Glove to be later used as weights in Neural Network.
4. Created Char Embedding Matrix of unique chars in our data using Glove to be later used as weights in Neural Network.
4. Performed analysis on Class Distribution and computed Class Weights to be later used in Neural Network.
5. Built a Word Embedded and Char Embedded Convolutional Neural Network (CNN) using a combination of Embedding, Conv1d, MaxPooling, Flatten, Dropout and Dense layers and implemented necessary callbacks(EarlyStopping, ModelCheckpoint and Tensorboard).
6. Achieved an Accuracy Score of 0.81 on Word CNN.
