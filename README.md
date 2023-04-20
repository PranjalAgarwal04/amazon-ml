# Product Length Prediction Model

In this hackathon, the goal is to develop a machine learning model that can predict the length dimension of a product. Product length is crucial for packaging and storing products efficiently in the warehouse. Moreover, in many cases, it is an important attribute that customers use to assess the product size before purchasing. However, measuring the length of a product manually can be time-consuming and error-prone, especially for large catalogs with millions of products.

You will have access to the product title, description, bullet points, product type ID, and product length for 2.2 million products to train and test your submissions. Note that there is some noise in the data.

## Task

- [ ] build a machine learning model that can predict product length from catalog metadata.

- [ ] Data collection and preparation: Collect a dataset that contains product metadata (e.g., product name, category, brand, etc.) and their corresponding lengths. You can collect this data from your own catalog or from a publicly available dataset. Then, you need to clean and preprocess the data, which may include removing missing values, converting categorical variables into numerical representations, and normalizing the data.

- [ ] Feature selection: Identify which features in your dataset are most relevant for predicting product length. You can use techniques such as correlation analysis or feature importance ranking to help you with this step.

- [ ] Model selection: Choose a machine learning algorithm that is appropriate for the problem you are trying to solve. In this case, since you are trying to predict a continuous variable (product length), regression models such as linear regression or decision trees may be suitable.

- [ ] Model training and evaluation: Split your dataset into training and testing sets, and train your chosen model on the training set. Evaluate the performance of your model on the testing set using metrics such as mean absolute error (MAE) or root mean squared error (RMSE).

- [ ] Hyperparameter tuning: Fine-tune the parameters of your model to improve its performance. This can be done using techniques such as grid search or random search.

- [ ] Deployment: Once you are satisfied with the performance of your model, you can deploy it in a production environment where it can be used to predict product lengths based on catalog metadata.

It is important to note that building a machine learning model requires a good understanding of the underlying statistical and mathematical concepts, as well as programming skills to implement the model in a programming language such as Python. Additionally, it is important to ensure that your model is fair and unbiased, and that it does not perpetuate any discriminatory practices.

## Dataset description

The dataset folder contains the following files:

- train.csv: 2249698 x 6
- test.csv: 734736 x 5
- sample_submission.csv: 734736 x 2

## The columns provided in the dataset are as follows

| Column name     | Description                                     |
| :---------:     | :--------:                                      |
| PRODUCT_ID      | Represents a unique identification of a product |
| TITLE           | Represents the title of the product             |
| DESCRIPTION     | Represents the description of the product       |
| BULLET_POINTS   | Represents the bullet points about the product  |
| PRODUCT_TYPE_ID | Represents the product type                     |
| PRODUCT_LENGTH  | Represents the length of the product            |

## Evaluation metric

```
score = max( 0 , 100\*(1-metrics.mean_absolute_percentage_error(actual,predicted)))
```

## Result submission guidelines

- The index is "PRODUCT_ID" and the target is the "PRODUCT_LENGTH" column.
- The submission file must be submitted in .csv format only.
- The size of this submission file must be 734736 x 2.
- Note: Ensure that your submission file contains the following:
- Correct index values as per the test file
- Correct names of columns as provided in the sample_submission.csv file

## Dataset

- [Dataset](https://s3-ap-southeast-1.amazonaws.com/he-public-data/datasetb2d9982.zip)

## Authors

- [@pranjal]()
- [@akanksha]()
- [@prajesh]()
