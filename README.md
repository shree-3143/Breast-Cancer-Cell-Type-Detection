# Breast Cancer Cell Type Detection
(This project won 1st Place in the ACT Young ICT Explorers (YICTE) Competition in Year 10 2023. This was also my Year 11 Semester 1 project)


<h3>Project summary:</h3>

My project is a Cell Type Identifier for Breast Cancer. I have created a model (using pre-existing models from Scikit-Learn) to detect cancerous cells. This project analyses the cell nuclei of cells sampled from an FNA (Fine-Needle Aspiration) and predicts whether or not the cell is cancerous based on the properties of the cell. 

<h3>About the dataset:</h3>

I have used the Breast Cancer Wisconsin (Diagnostic) Data Set for my project. This dataset contains properties of cell nuclei from 569 different patients. For each cell’s nucleus, 10 features are computed, with the mean, standard error, worst, and largest (the mean of the 3 largest values) also being recorded, giving 31 properties for each cell nucleus in total.!

Link to dataset: 
https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data

<h3>Programs and technologies used:</h3>

-	Google Colab (Hosted Jupyter Notebook Service)
-	Python
-	Different Libraries: NumPy, Pandas, MatPlotLib, Seaborn, Scikit-Learn
-	Models (from Scikit-Learn): Logistic Regression, Decision Tree Classifier, Random Forest Algorithm

<h3>Problem statement:</h3>


Breast Cancer is the most commonly diagnosed cancer amongst women in Australia. According to the National Breast Cancer Foundation, approximately 57 women are diagnosed with Breast Cancer every day, meaning over 20000 women are diagnosed with this cancer every year. 1 in 7 women are diagnosed with Breast Cancer in their lifetime. Currently, approximately one woman under the age of 40 is expected to die each week from breast cancer. In the last 10 years, breast cancer diagnosis has increased by 33%.


Although cell type detection is only a very small part of determining whether or not a tumor is “Malignant” and cancerous, correctly identifying cells within a tumor microenvironment provides oncologists an insight into how a patient’s immune system reacts to the tumor. Machine learning techniques can be used for automatic cell type detection. Such contributions to the classifications of tumors can ensure early diagnosis of breast cancer – meaning that symptomatic breast cancer patients can more likely be treated successfully. 

<h3>Design and features:</h3>

After cleaning, manipulating, exploring and visualizing the data, I split the data into training and testing data sets (75% of the dataset was dedicated to training and 25% of the dataset was dedicated to testing). 

The dependent dataset (Y) contained the diagnosis column – the target values – whether or not the patient has cancer. The independent dataset (X) contained data of the properties of each cell nucleus (essentially, the data used to achieve the target values).

After scaling the data to ensure all data was of the same magnitude, I trained the 3 models (from Scikit-Learn) on the training data. I found that the Decision Tree Classifier had the highest accuracy of the 3 models (100%) on the training data. I then proceeded to test this model (with the 3 models) on the testing data, using a confusion matrix, and found that the Random Forest Algorithm had the highest accuracy of the 3 models (98.6%) on the testing data.

Therefore, the Random Forest Algorithm was the model I decided to use the classify the cells (testing data, 25% of the dataset) as Malignant (cancerous) or Benign (non-cancerous).

<h3>Final prediction:</h3>

The final step to the project was printing the prediction of the data using the model. As I deduced that the Random Forest Algorithm had the highest testing accuracy, I printed the prediction of the data using this model. Essentially, now we are seeing if the prediction of the independent testing dataset matches the actual dependent testing dataset.

- 1 = Malignant cell
- 0 = Benign cell

<img width="801" alt="Screen Shot 2023-09-25 at 11 14 21 pm" src="https://github.com/shree-3143/Breast-Cancer-Cell-Type-Detection/assets/130221650/e6cb01c3-79ee-4ceb-820b-ac690069ea48">


The model is relatively accurate. There are only two cells that the model has identified incorrectly, one being a False-Positive and one being a False-Negative.

<h3>Graphs used:</h3>

**Correlation of Properties Heatmap (of first 10 properties):**

<img width="207" alt="image" src="https://github.com/shree-3143/Breast-Cancer-Cell-Type-Detection/assets/130221650/f75dd75e-16fd-4264-8cce-593aded028e4">



**Pair Plot (of first 3 properties):**

<img width="165" alt="image" src="https://github.com/shree-3143/Breast-Cancer-Cell-Type-Detection/assets/130221650/e9a51326-1dd2-44c9-98af-960da1e498d0">



**Pie Chart of Class Distribution:**

<img width="161" alt="image" src="https://github.com/shree-3143/Breast-Cancer-Cell-Type-Detection/assets/130221650/7b10e413-31b2-4801-b52e-d7976f65622b">



**Count Plot of Class Distribution:**

<img width="204" alt="image" src="https://github.com/shree-3143/Breast-Cancer-Cell-Type-Detection/assets/130221650/13928c0e-9a0d-492e-bb6c-4fc1cc8c9d23">






<h3>Referencing:</h3>

The tutorial I followed for this project was:


https://www.youtube.com/watch?v=NSSOyhJBmWY


This is his website:

https://randerson112358.medium.com/















