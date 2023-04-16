# IDS721-project4

An Object detection API using sagemaker and API gateway.

# Work Flow
![image](https://user-images.githubusercontent.com/33047941/230996578-224226ec-b11a-45a5-bdcc-05c97429a36b.png)

# Contents

- The .ipynb is the trainning script I used to train the model.
- The handler.py is the script I used as the lambda handler function.

# Steps
- Prepairing training data and uploaded to S3 storage
  - Downloading training data from http://ai.stanford.edu/~jkrause/cars/car_dataset.html, generating annotation data using devkit provided by Stanfor cars dataset.
  <img src="https://user-images.githubusercontent.com/33047941/231008018-1fb85207-7fab-44dd-b819-ca52617c1720.png" alt="Cute cat" width="70%" height="70%">

- Train and build model using Sagemaker
<img src="https://user-images.githubusercontent.com/33047941/232342244-f07a168d-f449-445c-a579-ba6098294f95.png" alt="Cute cat" width="70%" height="70%">


- Deployed the training model as an real-time hosted endpoint
![image](https://user-images.githubusercontent.com/33047941/232342373-de0e41f5-142e-4748-997e-5b1abde20cfc.png)


- Created a serverless lambda handler to invoke the sagemaker endpoint and create a REST API to trigger the lambda function.

![image](https://user-images.githubusercontent.com/33047941/232342437-82147599-a8da-412b-b909-20d90f0ccf20.png)


# Demo

- I randomly picked an image of benz from internet to test our API:
<img src="https://www.gravityautossandysprings.com/galleria_images/4193/4193_main_l.jpg" alt="Cute cat" width="50%" height="50%">

src: https://www.gravityautossandysprings.com/galleria_images/4193/4193_main_l.jpg

- Here is the result:

![image](https://user-images.githubusercontent.com/33047941/232342142-e7909795-c6b1-436a-ad33-1078688f000f.png)

As you can see, it gives Mercedes-Benz C-Class Sedan 2012 as the prediction.


