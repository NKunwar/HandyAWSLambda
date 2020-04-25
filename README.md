# HandyAWSLambda
AWS Lambda functions practice &amp; learning

Creating First lambda function steps:

Step 1: Create a Lambda project in eclipse and change the Input type from Object to String
	Step 1.1: Write unique name for your Lambda Handler class
	Step 1.2: Select the type of Lambda that needs to be created. The Lambda type is identified by the type of Input it is processing. Either select the available options from the list or if its none of the available list then choose Custom (say, if the Lambda is for Processing AWS Gateway which handles incoming HTTP requests from REST Clients & Browsers OR if its any other type of Lambda Functions)
Step 2: Create a S3 bucket
Step 3: Create a ROLE for Lambda => next Permissions => Select AWSLambdaBasicExecutionRole => Click Next Tags => Next: Preview => Give a Unique name to the Role 

Now when YOU will refresh your Eclipse Toolkit and then in the OUTLINE Tab YOU will see the newly created Role for your Lambda function

Step 4: Right click on Eclipse Code editor where your code is written then Go to AWS Lambda => Upload function to AWS Lambda 
	Step 4.1: Select the S3 region and a Unique lambda Function name (preffered name is same as Class Name) => Next
	Step 4.2: Select correct IAM Role (the same role which you created in Step 3)
	Step 4.3: Select correct S3 bucket name to upload your Lambda code to. => Finish

Step 5: To test your Function, Right Click => AWS Lambda => Run function on AWS Lambda
	Step 5.1: A pop-up window will appear where we have to add our Input, for now just send "" [Empty String] => Invoke
	
--------------------------------------------------------------------------
