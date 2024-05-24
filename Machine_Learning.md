The objective of this projet is to utilize a convolutional neural network (CNN) to identify and characterize the scratch generated on the polymeric surfaces.The CNN model is augmented with data generated using FEA and virtual reality-based scratch generation and visibility analysis. The trained CNN network then feeds the output to a reagression analysis for predicting scratch performance of a polymer based on its constitutive and optical properties.
<br><br>
In this regard, I trained a U-Net convolutional network for the task of segmenting and localizing surface scratches, the following process was followed:
<br><br>
## 1. Data Collection and Annotation
<br><br>
A dataset of images showing various surfaces with scratches was collected to cover a wide range of scenarios, lighting conditions, and scratch types.
Using LabelMe, an open-source annotation software, each image was carefully annotated to mark the scratches. The annotations were done by drawing precise polygons around each scratch, capturing the nuances of shape, size, and orientation.
<br><br>
## 2. Data Preparation
<br><br>
The JSON files from LabelMe were processed to extract the polygon coordinates for each scratch annotation.
These coordinates were used to create binary mask images where the scratches were marked in white (value 1) on a black background (value 0), matching the dimensions of the corresponding source images.
The original images and the generated binary masks formed a paired dataset, with each image having a corresponding mask to denote the location and shape of scratches.
<br> <br>
<img src="assets/img/Masking.JPG?raw=true" width="100%" height="100%">
<br> <br>
## 3. Model Configuration
<br><br>
A U-Net convolutional network was chosen for this task due to its proficiency in detailed image segmentation and its ability to capture fine features in images, such as surface scratches.
The network was configured with layers suitable for the size and complexity of the task, ensuring that it could handle the nuances of texture, contrast, and edge information present in the scratch data.
<br><br>
## 4. Training Process
<br><br>
The dataset was divided into training, validation, and test sets to evaluate the model's performance and generalize its capability to unseen data.
The U-Net model was trained using the training set, where it learned to predict the scratch locations and shapes by mapping the input images to their corresponding mask images.
Regular evaluation on the validation set helped in tuning the model parameters, preventing overfitting, and optimizing the learning rate and other hyperparameters.
<br><br>
## 5. Evaluation and Optimization
<br><br>
After training, the model's performance was evaluated using the test set to assess its ability to accurately segment and localize scratches on new, unseen images. One example of scratch detection is shown below.
<br> <br>
<img src="assets/img/Scratch_Detection.JPG?raw=true" width="100%" height="100%">
<br> <br>
## 6. Integration with Experiemntal Data
<br> <br>
The scratch normal load data from the scratch tester and length scale was integrated with the script. Now, the ML code can count the number of scratches, define their length and get the respective normal load at which scratch became visible using the experimental data and the scratch detection by CNN.
<br> <br>
<img src="assets/img/Scratch_Load.JPG?raw=true" width="100%" height="100%">
<br> <br>
## 7. Regression Analysis
<br> <br>
Next step is utilizing linear regression analysis to develop a weighted equation predicting Scratch Visibility Load. By analyzing the relationships between the dependent variable (Scratch Visibility Load) and the independent variables (Yield, Hardening and Friction), each predictor's influence can be identified statistically. This will allow for accurate forecasting of scratch visibility load based on these material properties and conditions, optimizing the scratch performance of polymers. For example, image below shows linear regression applied on CNN results and experimental data available for a small set.
<br> <br>
<img src="assets/img/Regression.png?raw=true" width="100%" height="100%">
<br> <br>
Till now model is trained only on scratches on black polycarbonate and TPO samples. This model will be expanded gradually to cover effect of color, gloss and texture also. More Results will be posted here soon....



