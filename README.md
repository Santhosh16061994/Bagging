# Bagging & Boosting

Bagging and boosting are both ensemble techniques in machine learning that aim to improve the performance of predictive models by combining multiple weaker models. While they share the goal of creating an ensemble of models, they differ in their approach and how they combine the individual models.

Bagging (Bootstrap Aggregating):
Bagging involves creating multiple models by training them on different subsets of the training data, obtained through bootstrapping (random sampling with replacement). Each model is trained independently, and the final prediction is obtained by aggregating the predictions of all models, typically through majority voting for classification problems or averaging for regression problems. The idea behind bagging is to reduce variance and overfitting by incorporating diverse models that are trained on different subsets of the data. Random Forest is an example of a bagging algorithm that employs decision trees as base models.

Boosting:
Boosting, on the other hand, involves iteratively training models in a sequential manner, where each subsequent model tries to correct the mistakes made by the previous models. Initially, all samples in the training set are given equal weights, and a base model is trained. The subsequent models focus on the samples that were misclassified by the previous models, assigning higher weights to those samples. This way, subsequent models pay more attention to the previously misclassified samples, gradually improving the overall prediction performance. The final prediction is obtained by aggregating the predictions of all models, often through weighted voting or weighted averaging. Examples of boosting algorithms include AdaBoost, Gradient Boosting Machines (GBM), and XGBoost.

Differences between Bagging and Boosting:
1. Approach: Bagging creates multiple models independently, each trained on a different subset of the data, while boosting trains models sequentially, with each model focusing on correcting the mistakes of the previous models.
2. Weighting: Bagging treats all samples equally during training, while boosting assigns higher weights to misclassified samples to give them more emphasis.
3. Aggregation: Bagging typically uses majority voting or averaging to aggregate predictions, while boosting uses weighted voting or weighted averaging, where more weight is given to the models that perform better.

In summary, both bagging and boosting are ensemble techniques that combine multiple models, but they differ in their training approach, sample weighting, and aggregation methods. Bagging aims to reduce variance and overfitting, while boosting focuses on improving the model's ability to handle difficult-to-classify samples. Both techniques have been successful in improving the performance and robustness of predictive models in various machine learning tasks.
