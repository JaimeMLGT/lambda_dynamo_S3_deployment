
# Project Overview

In this project i will use cloudformation template to build the entire infrastructure of multiple AWS resources based on a previous assessment that i reciently had. 

The services that i will use will be the following ones:

* Cloudformation
* DynamoDB
* S3 Bucket 
* SES 
* Lambda
* EventBridge 
* IAM

## STAR method Explanation

The **situation** was to create an application based on DynamoDb and interconnected with different AWS elements for an access test.

The **task** here was about a couple of dynamoDB tables called RA_totales and VR_totales which should store the number of products based on their respective types, Augmented Reality (RA) or Virtual Reality (VR).
You could build any number of tables based on prefix RA or VR and in case that table would have elements inside ,this program will print the number of items , date and name of the elements of each type. 

I should store the file inside a bucket S3 in json format, and as a reminder send an authorized email (previously integrated in AWS) to a  certain email address. The execution of the entire program should be programmed , with 5 mins of delay between each new iteration.

The **Action** that i did , was mainly use something different and creative with quick deployment as AWS Cloudformation service. I decided to use Python as the lenguage to make the lambda function, SES to send the message based on AWS, S3 was mandatorial so i couldn't choose other option here , and the IAM execution roles for the Lambda (SES,S3,DynamoDB access).For the 5 min program execution my chooice was EventBridge because when i studied my solution architect exam i could practice a little bit with it and was a preference that i had.To have it in a more autonomous way , i built some custom tables for each type to have something very quick to test in time. 

As a **Result**, I could make this work and not only that , i made it in a different way as it was initialy thought and this gave me a lot of points in comparation to other candidates that were pushing for the same role. They congrats me and if you want to know the end of the story don't be shy and reach me out , i will be more than happy to tell you the final decision. 

## End Credits

This program is ready to use and set up if you wanna to give it a try , so feel free to use it with responsability and don't forget to  write your own source_email and destination_email. 



