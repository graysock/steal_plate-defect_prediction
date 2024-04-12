# steal_plate-defect_prediction
This project predicts the type of defect on steal plates
Data set comes from Kaggle play ground series.
Overall score is based on the average AUC score. 
Final results: .888 AUC score. 
Overall the model was underpredicting the `Other_Faults` class so I added a bias to this class to increase its predition counts.
Each class was very unbaanced making it difficult to predict but overall the results were good. 

## Challenges 
First I was happy I wrote a function that retrained and refit for each class type. The model also added the predicted classes previously into account which was great because the class that had the most instances `Other_Faults` wasnegatively orrolated with `K_Scatch` another one of the predicted class defects. Adding this feature to the model significantly increased its predicting power for the `Other_Faults` class.
