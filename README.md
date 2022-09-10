AWS-S3 bucket to SageMaker

![image](https://user-images.githubusercontent.com/111189874/189472578-dd814e87-f81c-4c32-a9ce-fc2ee2df9f65.png)





** Requirements:
->we have to create a AWS account 
->numpy
->pandas


1. About AWS S3 bucket:
* Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can use Amazon S3 to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides management features so that you can optimize, organize, and configure access to your data to meet your specific business, organizational, and compliance requirements.

2. How Amazon S3 works:
* Amazon S3 is an object storage service that stores data as objects within buckets. An object is a file and any metadata that describes the file. A bucket is a container for objects.

* To store your data in Amazon S3, you first create a bucket and specify a bucket name and AWS Region. Then, you upload your data to that bucket as objects in Amazon S3. Each object has a key (or key name), which is the unique identifier for the object within the bucket.

* S3 provides features that you can configure to support your specific use case. For example, you can use S3 Versioning to keep multiple versions of an object in the same bucket, which allows you to restore objects that are accidentally deleted or overwritten.

* Buckets and the objects in them are private and can be accessed only if you explicitly grant access permissions. You can use bucket policies, AWS Identity and Access Management (IAM) policies, access control lists (ACLs), and S3 Access Points to manage access.

3. Creating a S3 bucket:
![image](https://user-images.githubusercontent.com/111189874/189471922-facd56f7-c7c8-43c3-b639-34973754f860.png)

4. About the sagemaker:
* To make it easier to get started, Amazon SageMaker JumpStart provides a set of solutions for the most common use cases that can be deployed readily with just a few clicks.
* Prepare, build, train, and deploy high-quality machine learning models quickly by bringing together a broad set of capabilities purpose-built for machine learning.


5. Creating the notebook instance:
 step1: To create a notebook instance, use either the SageMaker console or the CreateNotebookInstance API.
 * In the Notebook instance name and tab, type a suitable name and tag for your notebook instance.
 
 ![image](https://user-images.githubusercontent.com/111189874/189472366-f63e65bf-d8c0-48a7-ab72-9c56f839b1a8.png)

step2: Create an IAM Role
* Next, specify the IAM role for the SageMaker model. You can either select an existing IAM role in your account or Create a new role.

![image](https://user-images.githubusercontent.com/111189874/189472396-d0c51ee3-c015-4eb7-a385-618a3f94ecc4.png)

step3: Finally, click on the Create notebook instance.

![image](https://user-images.githubusercontent.com/111189874/189472427-2073be60-2021-4835-9c69-dc74cc89fbd1.png)


outputs:

![image](https://user-images.githubusercontent.com/111189874/189472460-d39e7137-6486-4800-9f82-afbfd5fbdc97.png)





![image](https://user-images.githubusercontent.com/111189874/189472112-7f06eb0b-5e1b-447f-a111-32fed8073bed.png)



6. Builds:
* It provides more than 15 widely used ML Algorithm for training purpose.
* It gives the capability to select the required server size for our notebook instance.
* A user can write code (for creating model training jobs) using notebook instance.
* Choose and optimize the necessary algorithm, such as
-> K-means
-> Linear regression
-> Logistic regression
* AWS SageMaker helps developers to customize Machine Learning instances with the Jupyter notebook interface.

7. Test and Tune :
* Set up and import required libraries.
* Define a few environment variables and manage them for training the model.
* Train and tune the model with Amazon SageMaker.
* SageMaker implements hyperparameter tuning by adding a suitable combination of algorithm parameters.
* SageMaker uses Amazon S3 to store data as it’s safe and secure.
* SageMaker uses ECR for managing Docker containers as it is highly scalable.
* SageMaker divides the training data and stores in Amazon S3, whereas the training algorithm code is stored in ECR
 Later, SageMaker sets up a cluster for the input data, trains, and stores it in Amazon S3 itself.
 
 8. Deploy:
* Once tuning is done, models can be deployed to SageMaker endpoints.
* In the endpoints, a real-time prediction is performed.
 Now, evaluate your model and determine whether you have achieved your business goals.
 
 




















