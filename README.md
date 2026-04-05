# Feature-Engineering
1. Accuracy  
Comparing different values of top_k (3, 5, 6) against the base top_k=10 showed that increasing the number of categories resulted in poorer outcomes for the algorithm.
Top_k = 3: The most accurate result was 40.18%.

Baseline (top_k = 10): Accuracy was 39.36%.

Top_k = 5: Accuracy was 39.26%.

Top_k = 6: Accuracy was 39.08%.
Conclusion: According to the above data, the most optimal top_k parameter for our case should be 3. With only 3 elements in the category (Item_Name), we got rid of the rare objects that confused the algorithm.
2. Features importance
Based on the analysis above, there were changes in the significance of the features:

Significant factors: Just like earlier observed, Unit_Price and Quantity are significant for predicting the target class in all scenarios.

Impact on Item_Name_reduced:

For top_k=3: The factor "Item Name" can be considered significant as well because despite being a very simple factor, it achieves high accuracy.

For top_k=10: In contrast to the scenario top_k=3, the model has more defined labels. However, the accuracy in this scenario is lower compared to top_k=3.
