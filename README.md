# Feature-Engineering
1. Accuracy  
Comparing different values of top_k (3, 5, 6) against the base top_k=10 showed that increasing the number of categories resulted in poorer outcomes for the algorithm.
Top_k = 3: The most accurate result was 40.18%.

Baseline (top_k = 10): Accuracy was 39.36%.

Top_k = 5: Accuracy was 39.26%.

Top_k = 6: Accuracy was 39.08%.
Conclusion: According to the above data, the most optimal top_k parameter for our case should be 3. With only 3 elements in the category (Item_Name), we got rid of the rare objects that confused the algorithm.

2. Features importance
This is how the model sorted out the factors by their importance in all runs:

Top factors: Unit_Price and Quantity are the top features in each of the experiments conducted. They played an important role in almost all decisions taken by the model.

Impact on Item_Name_reduced:

top_k=3: The model was able to obtain maximum accuracy using this feature because it used very few labels. Thus, we see how simplicity is more valuable than complexity.

In the cases top_k=10&6, the model had to consider names more carefully than before, but due to poor accuracy, we see how these additional details were a hindrance rather than assistance.

For top_k=5, the feature remained among the top three features and formed an integral part of predictions made by the model.
