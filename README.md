# Credit_Risk_Analysis

## Purpose
The purpose of this analysis is to determine the best machine learning model for analyzing credit risk with this dataset. It should not be taken as an analysis of credit risk in general. Different types of credit or different datasets may yield different results.

## Accuracy and Precision of 6 different models

### 1. Random Oversampling
SUMMARY: This model performed the best of the simple models, but still was not terribly impressive. The balanced accuracy score was just under 66%. All of the models had the same precision score (0.99), but with low sensitivity. The sensitivity for this model was 0.64


![image](https://user-images.githubusercontent.com/84299125/137942544-28ac9d7d-cc38-49dd-ac06-807a59c6b03e.png)
![image](https://user-images.githubusercontent.com/84299125/137942916-e5d3eb1b-bbaa-4071-a1ad-41758970767f.png)


### 2. SMOTE Oversampling
SUMMARY: This model had the same precision and sensitivity as the random oversampling, but a slightly lower balanced accuracy score at 63%.

![image](https://user-images.githubusercontent.com/84299125/137943065-0bdea355-98fa-42bd-8276-b0b67b74d142.png)
![image](https://user-images.githubusercontent.com/84299125/137982686-bb9a14c9-5465-408e-9a31-75611ab9ab08.png)


### 3. Cluster Centroids Undersampling
SUMMARY: This was the worst-performing model. A balanced accuracy of just over half, with recall less than half. I would definitely not recommend this model for this dataset.

![image](https://user-images.githubusercontent.com/84299125/137983120-0e1bf5af-6c69-4c1c-a770-4c2889ff8e42.png)
![image](https://user-images.githubusercontent.com/84299125/137983205-cce989e6-642b-4e0d-8656-177175b51d2c.png)


### 4. Combination Sampling with SMOTEEN
SUMMARY: This was second best of the simple models with a balanced accuracy of 0.63 and recall of 0.58. 

![image](https://user-images.githubusercontent.com/84299125/137983724-179c7431-cbc0-4af7-8bbe-8002c2ae839f.png)
![image](https://user-images.githubusercontent.com/84299125/137983798-2561513c-9274-41d6-bb0f-b135a90b6819.png)


### 5. Balanced Random Forest Classifier
SUMMARY: This model performed significantly better than any of the simple models. The balanced accuracy was 79% with a recall of 0.87. Precision remained at 0.99.

![image](https://user-images.githubusercontent.com/84299125/137983882-2f7044e8-1e4e-4422-a9bd-0d9142400093.png)
![image](https://user-images.githubusercontent.com/84299125/137984300-517cee3d-8e5c-43a8-a7d8-a7f739d86e36.png)


### 6. Easy Ensemble Classifier
SUMMARY: Highest overall scores were seen in this model. The balanced accuracy was 93%, with a recall of 0.94. 

![image](https://user-images.githubusercontent.com/84299125/137984384-962f776b-f852-4089-8d04-7a42464ed194.png)
![image](https://user-images.githubusercontent.com/84299125/137984480-9b95a016-a9ff-424d-890f-2fcb854fc762.png)

## RECOMMENDATION

After running all of these models, I would recommend the Easy Ensemble Classifier. No other model had a sufficiently high balanced accuracy score. In addition, it was a simpler model than some of the others. 
