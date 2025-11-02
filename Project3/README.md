KNN Classification on Unknown Dataset

    This project demonstrates the application of K-Nearest Neighbors (KNN) for classification on a dataset with unknown feature meanings. The dataset contains numerical features with random labels and a target variable TARGET CLASS.

Steps Performed

    Data Overview:

        The dataset features are unknown, so no detailed exploratory data analysis was performed.
        A simple pairplot was created to get a rough idea of feature relationships with the target.

    Data Preprocessing:

        Standardized numerical features using StandardScaler, so all features have mean = 0 and std = 1.
        Created a scaled DataFrame df_scaled with standardized values.

    KNN Modeling:

        Trained a KNN classifier with initial k=1 neighbors, which produced lower accuracy (0.72).
        Tuned the number of neighbors by testing k from 1 to 40.

        Found that k=31 gives the best performance:

        Accuracy: 0.84
        Confusion Matrix:

            [[123  29]
            [ 19 129]]


    Conclusion

        Even with unknown feature meanings, KNN can effectively classify the target variable after feature standardization.
        Proper tuning of k significantly improves model performance.
        Standardization of features is essential for distance-based algorithms like KNN.

    Tools Used

        Python: Pandas, NumPy
        Seaborn & Matplotlib: Basic visualization
        Scikit-learn: StandardScaler, KNeighborsClassifier