# Heart_disease_diagnosis_UsingSVM
In this work, we used dataset from https://www.geeksforgeeks.org/machine-learning/dataset-for-classification/, which contains 569 instances with 30 features such as radius, texture, perimeter, and area of the nuclei. Main idea for this work using this features as input to Support Vectore Machine (SVM) algorithm to identifying the heart disease and predict type of tumor as  a benign or a malignant.
This dataset was very clean and balanced data and all data was a numerical data, we tried to apply standard scalar to normalize the data but it affected on the decision boundaries, when we used RBF kernel. finally we just applied feature Principal Component Analysis (PCA) to reduce the dimentionality to the feature to facilitate the drawing of the decision boundaries, when we used SVM with linear and Radial Basis Function (RBF) kernels. then we split data into training and testing. then we applied SVM with two Kernel to comparing between the performance using each kernel.

Our results were very close using the two kernels, were Linear Kernel achieved accuracy of 70% and RBF 69%.

Next image shows the decision boundaries using linear kernel, that represint the decision boundary is a straight line
<img width="644" height="405" alt="image" src="https://github.com/user-attachments/assets/5a19a93e-11ae-4ba7-a048-718d53667f67" />
# Linear kernel: finds a straight-line (hyperplane) decision boundary. Suitable when data is approximately linearly separable.

While the next image shows  the decision boundaries using RBF to capture complex, non-linear patterns.
<img width="656" height="400" alt="image" src="https://github.com/user-attachments/assets/182034f5-a5be-43b0-8c3e-94355534632f" />
#  RBF Maps data implicitly into a high-dimensional feature space. Allows non-linear decision boundaries and gamma controls the influence of each training sample.


Finally, we concluded that the best one was the simple RBF , because the two kernels reached to very close resuts, but the nature of the problem is a non-linear problem and that is the work of the RBF.





