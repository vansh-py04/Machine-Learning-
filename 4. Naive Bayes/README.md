Naive Bayes is a simple yet powerful probabilistic classifier based on Bayes' theorem with the "naive" assumption of feature independence. Despite its simplicity, Naive Bayes often performs surprisingly well in practice, especially for text classification and other high-dimensional datasets.

### Bayes' Theorem:

Bayes' theorem describes the probability of a hypothesis given evidence and prior knowledge. Mathematically, it is represented as:

\[ P(h | e) = \frac{P(e | h) \cdot P(h)}{P(e)} \]

![image](https://github.com/vansh-py04/Machine-Learning-Algorithms-from-Scratch/assets/128248352/4ca3e683-5dd8-439f-b666-0872497d43e8)

Where:
- \( P(h | e) \) is the posterior probability of hypothesis \( h \) given evidence \( e \).
- \( P(e | h) \) is the likelihood of evidence \( e \) given hypothesis \( h \).
- \( P(h) \) is the prior probability of hypothesis \( h \).
- \( P(e) \) is the probability of evidence \( e \).

### Naive Bayes Classifier:

In the context of classification, Naive Bayes assumes that the presence (or absence) of each feature is independent of the presence (or absence) of any other feature, given the class label. This simplifies the computation of the likelihood term and leads to a computationally efficient classifier.

#### Algorithm Steps:
1. **Training**:
   - During training, Naive Bayes calculates the prior probability of each class and the conditional probability of each feature given each class using the training data.
   
2. **Prediction**:
   - To predict the class of a new instance, Naive Bayes computes the posterior probability of each class given the features of the instance using Bayes' theorem.
   - Since the evidence \( e \) is constant for all classes, the classifier compares the posterior probabilities and assigns the class with the highest probability to the new instance.

#### Types of Naive Bayes Classifiers:
- **Gaussian Naive Bayes**:
   - Assumes that the continuous features follow a Gaussian distribution.
- **Multinomial Naive Bayes**:
   - Suitable for discrete features (e.g., word counts in text classification).
- **Bernoulli Naive Bayes**:
   - Similar to Multinomial Naive Bayes but considers binary features (presence or absence of a feature).

### Hyperparameters:
- **Smoothing Parameter (Alpha)**:
   - Used to handle zero probabilities when a feature does not occur with a particular class in the training data.
   - Common smoothing techniques include Laplace smoothing (additive smoothing) and Lidstone smoothing.

### Pros and Cons:
- **Pros**:
   - Simple and easy to implement.
   - Efficient and scalable, especially for high-dimensional data.
   - Performs well with small training datasets.
- **Cons**:
   - Strong feature independence assumption, which may not hold in real-world datasets.
   - Sensitivity to irrelevant features.
   - Can be outperformed by more complex models when the independence assumption is violated.

### Visualization:
![image](https://github.com/vansh-py04/Machine-Learning-Algorithms-from-Scratch/assets/128248352/5b9a1429-1e3e-43fc-8afb-4389e7eb23d8)
