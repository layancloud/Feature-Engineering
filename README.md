# Feature-Engineering
1. Accuracy  
Our review of the correct data reveals an unexpected yet interesting pattern: the accuracy does not improve as the number of categories increases. In fact, it is highest with the fewest categories.  

Top_k = 3: Accuracy of 40.18%.

Baseline (top_k = 10): 39.36% Accuracy.

Top_k = 5: 39.26% Accuracy.

Top_k = 6: Lowest Accuracy was of 39.08%.

Conclusion: It is important to note that reducing the number of item categories to only the top three increased the accuracy of the model.This suggests that adding more item names, from 4 to 10, may have confused or distracted the Random Forest model.This suggests that adding more item names, from 4 to 10, may have confused or distracted the Random Forest model.
2. Features importance
Based on the analysis above, there were changes in the significance of the features:

Significant factors: Just like earlier observed, Unit_Price and Quantity are significant for predicting the target class in all scenarios.

Impact on Item_Name_reduced:

For top_k=3: The factor "Item Name" can be considered significant as well because despite being a very simple factor, it achieves high accuracy.

For top_k=10: In contrast to the scenario top_k=3, the model has more defined labels. However, the accuracy in this scenario is lower compared to top_k=3.
