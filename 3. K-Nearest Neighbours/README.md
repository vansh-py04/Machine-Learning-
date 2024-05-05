### K-Nearest Neighbors (KNN) for Classification:

KNN is a simple yet powerful non-parametric classification algorithm. It classifies new data points based on the majority class of their K nearest neighbors in the feature space.

#### Algorithm Steps:
1. **Training**:
   - During the training phase, KNN stores all available data points and their corresponding class labels.
   
2. **Prediction**:
   - To predict the class of a new data point, the algorithm calculates the distances between the new point and all training data points using a distance metric such as Euclidean distance.
   - It then selects the K nearest data points (neighbors) based on these distances.
   - The predicted class for the new data point is determined by a majority vote among its K nearest neighbors.
   
#### Hyperparameter: 
- **K (Number of Neighbors)**:
   - The choice of K is a crucial hyperparameter in KNN. A smaller value of K makes the model sensitive to noise, while a larger value of K makes the decision boundary smoother but may lead to the inclusion of unrelated data points.

![image](https://github.com/vansh-py04/Machine-Learning-Algorithms-from-Scratch/assets/128248352/fec06fa9-35ab-4353-9b49-b1c8f08455dd)

### K-Nearest Neighbors (KNN) for Regression:

KNN can also be used for regression tasks, where the goal is to predict a continuous target variable rather than a class label.

#### Algorithm Steps:
1. **Training**:
   - Similar to classification, during training, KNN stores all available data points and their corresponding target values.
   
2. **Prediction**:
   - To predict the target value for a new data point, the algorithm calculates the distances between the new point and all training data points.
   - It then selects the K nearest data points (neighbors) based on these distances.
   - The predicted target value for the new data point is typically the average (mean or median) of the target values of its K nearest neighbors.
   
#### Hyperparameter:
- **K (Number of Neighbors)**:
   - As in classification, the choice of K is critical in regression. A smaller value of K may lead to a more flexible model but could be sensitive to outliers, while a larger value of K may lead to a smoother regression curve but may not capture local variations in the data effectively.

![image](https://github.com/vansh-py04/Machine-Learning-Algorithms-from-Scratch/assets/128248352/5246ebb0-4114-4d88-a19d-0fb2f3f30dfc)

### Pros and Cons:
- **Pros**:
   - Simple and easy to understand.
   - No assumption about the underlying data distribution.
   - Can be effective for both classification and regression tasks.
- **Cons**:
   - Computationally expensive during prediction, especially with large datasets.
   - Sensitivity to the choice of K and the distance metric.
   - Not suitable for high-dimensional data due to the curse of dimensionality.
