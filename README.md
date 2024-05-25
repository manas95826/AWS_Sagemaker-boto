## SageMaker XGBoost Model Deployment

This repository contains code for deploying an XGBoost model using Amazon SageMaker. The model is trained on the bank marketing dataset to predict whether a client will subscribe to a term deposit or not.

### Contents:

1. **Importing Important Libraries**: The necessary libraries are imported for the deployment process.

2. **Creating S3 Bucket**: The script creates an S3 bucket to store the dataset and trained model artifacts.

3. **Downloading The Dataset And Storing in S3**: The dataset is downloaded from a provided URL and stored in the previously created S3 bucket.

4. **Train Test Split**: The dataset is split into training and testing sets.

5. **Saving Train And Test Into Buckets**: The training and testing data are saved into separate folders within the S3 bucket.

6. **Building Models XGBoost- Inbuilt Algorithm**: An XGBoost model is built using SageMaker's built-in algorithm.

7. **Deploy Machine Learning Model As Endpoints**: The trained model is deployed as an endpoint using SageMaker.

8. **Prediction of the Test Data**: The deployed model is used to make predictions on the test data.

9. **Deleting The Endpoints**: Once the predictions are made, the deployed endpoint and associated resources are deleted to avoid unnecessary costs.

### Instructions:

1. Clone the repository.

2. Ensure you have an AWS account and appropriate permissions set up.

3. Install the required libraries specified in the `requirements.txt` file.

4. Update the `bucket_name` variable in the script to a unique name for your S3 bucket.

5. Run each cell in the Jupyter Notebook or execute the script.

6. Follow the instructions printed in the console for each step of the deployment process.

7. After making predictions, ensure to delete the endpoints to avoid unnecessary charges.

### Notes:

- Ensure proper configuration of AWS IAM roles and permissions.
- Monitor AWS resources to avoid unnecessary costs.
- Customize hyperparameters and model configurations as per your requirements.
- For detailed explanations, refer to the comments in the code cells of the Jupyter Notebook.

For any issues or queries, feel free to raise an issue in the repository or contact the repository owner.
