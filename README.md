# CMSC 35300 Project: Gesture Classification and Prediction

## Team Members
- Lan Gao
- Sam Cong
- Yun Ho 

## Dataset: Sign Language Digits Dataset
For this project, we used an [open-source dataset](https://github.com/ardamavi/Sign-Language-Digits-Dataset) called Sign Language Digits Dataset, which contains 2180 images of hand signs corresponding to digits (0-9) in American Sign Language. The raw dataset contains 2180 photos (each one is 100x100 pixels) of hand signs, which were classified into 10 classes. The raw images will undergo several preprocessing steps, including image resizing to a fixed dimension (specifically, 64x64 pixels), label assignment (via one-hot encoding), and normalization of pixel values to enhance contrast in grayscale data.

## Task 1: Sign Language Digits Prediction
We employed three traditional machine learning algorithms—k-nearest neighbors (KNN), random forest, and support vector machines (SVM)—to classify sign language digits based on image data. The process began by utilizing the image feature matrix as the input variable (X) and the corresponding ground truth labels as the target variable (y). To ensure robust model evaluation, we implemented K-fold cross-validation alongside performance assessment on a separate testing dataset. This approach facilitated the comparison of the predictive capabilities of each algorithm under consistent evaluation conditions.

## Task 2: Sign Language Digits Completion
We reconstructed the lower half of each image based on the upper half. Specifically, the goal was to predict the missing lower half leveraging information from the upper half, allowing the model to “complete” the image of each sign language digit. To achieve this, we experimented with various approaches, including ridge regression, principal component regression, and kernel ridge regression. Furthermore, we evaluated and compared model performance using metrics such as mean squared error (MSE), Structural Similarity Index Measure (SSIM), and Peak Signal-to-Noise Ratio (PSNR). Finally, we explained the differences in model performance and suggested potential ways to improve performance.
