# Lampda
## Description of How to use my Lambda.
1. Set Up Your AWS Environment
2. Create an S3 Bucket
3. Create a Lambda Function
* Go to the AWS Management Console and navigate to the Lambda service.
* Click on "Create function" and choose the option to author from scratch.
* Choose a name for your function and choose an execution role with permissions to access S3.
Write your Lambda function code to process the image uploads and update the images.json file. You can use the Boto3 library to interact with S3.
4. Write Lambda Function Code:
* In your Lambda function, you'll need to:
* **a.** Trigger the function when an object is uploaded to the S3 bucket.
* **b.** Download the images.json file from the S3 bucket (if it exists).
* **c.** Parse the JSON data to update or create an array of image objects.
* **d.** Extract metadata from the uploaded image (name, size, type, etc.).
* **e.** Append or update the metadata object to the array.
* **f.** Upload the updated images.json file back to the S3 bucket.
5. Test Your Lambda Function
6. Configure S3 Event Trigger
7. Deployment and Monitoring

## Description of any Issues I encountered

## Link to images.json file
* **My Lampda:** https://us-west-1.console.aws.amazon.com/lambda/home?region=us-west-1#/functions/myGreatLambda?tab=configure
* **My S3Bucket:** https://us-west-1.console.aws.amazon.com/s3/buckets/mycodefellowsbucket?region=us-west-1&bucketType=general&tab=objects
* **My File:** s3://mycodefellowsbucket/output/images.json
