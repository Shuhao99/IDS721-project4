# IDS721-project4

An Object detection API using sagemaker and API gateway.

# Work Flow
![image](https://user-images.githubusercontent.com/33047941/230996578-224226ec-b11a-45a5-bdcc-05c97429a36b.png)

# Steps
- Prepairing training data and uploaded to S3 storage
  - Downloading training data from http://ai.stanford.edu/~jkrause/cars/car_dataset.html, generating annotation data using devkit provided by Stanfor cars dataset.
  - ![image](https://user-images.githubusercontent.com/33047941/231008018-1fb85207-7fab-44dd-b819-ca52617c1720.png)

- Train and build model using Sagemaker
- Deployed the training model as an real-time hosted endpoint
- Created a serverless REST API
- Deploy API and tesing use curl

# Demo
