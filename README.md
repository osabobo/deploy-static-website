# Deploy a static website using AWS CodePipeline S3 and GitHub 


## Objective
In this project, i deployed a static website via AWS codepipeline. Below is the architectural diagram that details how to accomplish this task.



##  Project Architectural Diagram

![Untitled Diagram (12)](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/a40b4a8e-f722-4aef-b774-83ba27fe90b2)


## Steps taken to complete this project:

## Step 1: Upload/Push static web files to your GitHub Repo

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/836b11ce-29b4-4567-bead-9f085813c75c)



## Step 2: Create a S3 bucket and also Upload the static web files


![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/849f8cd9-b16a-40e7-8bb6-018b2ef761f3)


## Step 3: Create a CloudFront distribution and restrict access to S3 bucket content with OAI


![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/6a2e021e-1f89-4673-8d76-fed42b018e90)

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/89602494-8378-45dd-890c-4ced1e38c39c)

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/a9194e18-840b-4832-adb1-ebc7d1832fc3)

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/e7bc019c-edc5-47b5-a119-eaedacafbe2d)

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/cc043983-11c3-4482-9791-6ab942acbf97)

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/22e70da8-1e7b-46e7-bc3a-2ab45512115b)


## Step 4: Copy and paste the Cloudfront distribution domain name on a browser to access the website

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/500a1fee-4714-45cd-939a-5d3f8f6c9eff)

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/d3c53820-7479-477e-b872-cd1accbdc255)


## Step 5:  Implementing CI/CD through AWS CodePipeline

### a.Connect GitHub Account to CodePipeline


![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/815c0a99-e9c4-414a-8240-6185c343b16a)

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/80e175df-55aa-4320-9544-86e0edbda7f4)


### b.Configure CodePipeline and deploy CI/CD pipeline

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/2f55f14c-a7ac-46e6-8beb-44dc853510e6)

### Skip the build stage


![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/df7f8ab8-7367-4eac-9574-c278fb60cbd8)



Review the pipeline, then proceed to “Create pipeline”. Wait for the pipeline to be created.



![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/b95c2056-a358-4692-8a9c-54679f9278c4)



Yessssssssss!!!!!!!! the pipeline has been created, next we need to verify it.


## Step 6: Verify functionality of CI/CD Pipeline

Go to the github repo and edit any file, in my case i will edit the Readme file, once that is done, you will notice the pipeline is triggered, 


![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/05d1e8aa-6d4b-4c8f-b464-11032b064a48)

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/99c13783-2ab6-4787-9b09-a989069a2a17)


### a: and if you check the s3 bucket, you will find that the readme file has been added

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/868261f3-d373-47b9-a137-b772a79eb1dc)




## Finally, paste the domain name of the cloudfront distribution on a browser to access the website

![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/edb65cd2-d565-41c4-a722-46e0afc69541)


Yes the website can still be acessed, click on the "tell me more" button to see more


![image](https://github.com/georgeonalo/Deploy-a-static-website-using-AWS-CodePipeline-S3-and-GitHub-2/assets/115881685/0ba41b76-34d0-491e-9cbe-6ddb705c219f)




## Conclusion

In conclusion, if you follow all the steps mentioned above, you will succeed in deploying a any static website with AWS Codepipeline using Github and S3 bucket.













