## 1. Compute the value of the “good” model A below, relative to the default model.

How much greater or smaller is it?

Remember that the cost of using the model must be factored in.

Assume that the cost of using the good model is $40, while the cost of using the default model is $10.

### a. The Profit Matrix

This matrix defines the financial impact of every classification decision.

|                     | Predicted Positive | Predicted Negative |
|---------------------|-------------------:|-------------------:|
| Actual Positive     | TP: +$100          | FN: -$500          |
| Actual Negative     | FP: -$50           | TN: +$25           |

### b. Model Performance Matrices

The following matrices show the probability \(P\) of each outcome for the two models.

### Default Model

This model struggles with a high False Negative rate, which is particularly dangerous given our profit matrix.

|                     | Predicted Positive | Predicted Negative |
|---------------------|-------------------:|-------------------:|
| Actual Positive     | 0.40 (TP)          | 0.10 (FN)          |
| Actual Negative     | 0.20 (FP)          | 0.30 (TN)          |

### Good Model

This model is more precise, successfully shifting probability away from the "error" cells (FN and FP) and into the "correct" cells (TP and TN).

|                     | Predicted Positive | Predicted Negative |
|---------------------|-------------------:|-------------------:|
| Actual Positive     | 0.45 (TP)          | 0.05 (FN)          |
| Actual Negative     | 0.10 (FP)          | 0.40 (TN)          |

## 2. Design a scenario in which there are two distinct models, with different confusion matrices, all four values are different between the two models, and different accuracies, but where the two models generate exactly the same profit.

Do not use the same scenarios from the text.

Assume that the two models cost the same amount to use.

## 3. Suppose you are using the Top-K method where you can only address K = 10 items with the highest probability threshold.

Specifically rank items by predicted probability. Consider at most the top $K = 10$. Address an item only if the expected value of addressing it exceeds the expected value of not addressing it.

Describe a scenario where you would address less than 10 items and another in which you would address exactly 10.

Show the confusion matrices and profit for each.
