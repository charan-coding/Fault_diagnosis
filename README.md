Overview

Early detection and diagnosis of faults in synchronous generators are crucial for ensuring operational efficiency, quality assurance, and predictive maintenance. Several fault diagnosis techniques have been explored in the past, but this research implements a data-driven machine fault diagnosis system using empirical mode decomposition (EMD) and machine learning algorithms to improve accuracy.

Methodology

This work explores the application of Empirical Mode Decomposition (EMD) for breaking down current signals into Intrinsic Mode Functions (IMFs), which are analyzed for fault diagnosis. Machine learning techniques, including Convolutional Neural Networks (CNNs), Dense Neural Networks (DNNs), Support Vector Machines (SVMs), Random Forest Classifiers (RFCs), and K-Nearest Neighbors (KNNs), were used to classify faults effectively.

Performance Metrics & Results

We implemented a baseline model using raw machine data, achieving the following accuracy results:

CNN-based models:

R Phase: 90.42%

Y Phase: 90.59%

B Phase: 91.03%

DNN-based models:

R Phase: 91.25%

Y Phase: 91.34%

B Phase: 90.42%

SVM on raw data:

R Phase: 89.51%

Y Phase: 90.12%

B Phase: 90.32%

IMF and Bottleneck Feature Extraction

By using EMD and extracting bottleneck features from the IMFs, we significantly improved accuracy:

RFC Classifier:

R Phase: 95.42%

Y Phase: 94.86%

B Phase: 92.02%

KNN Classifier:

R Phase: 94.85%

Y Phase: 94.21%

B Phase: 93.09%

SVM on IMFs:

R Phase: 92.22%

Y Phase: 92.47%

B Phase: 92.53%

By combining IMF 1 and 2, we observed the highest improvement:

RFC on IMF 1 & 2:

R Phase: 95.16%

Y Phase: 93.32%

B Phase: 94.70%

KNN on IMF 1 & 2:

R Phase: 95.28%

Y Phase: 94.57%

B Phase: 94.85%

SVM on IMF 1 & 2:

R Phase: 83.24%

Y Phase: 84.25%

B Phase: 85.91%

Conclusion

Applying EMD and bottleneck feature extraction significantly improves classification accuracy over raw data models.

The combination of IMF 1 and 2 consistently produced the best results, particularly when classified using Random Forest (RFC) and KNN models.

The proposed system outperforms traditional machine learning models and provides a robust framework for early fault detection in synchronous generators.
