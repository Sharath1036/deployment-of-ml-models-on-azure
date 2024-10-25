# Deployment of ML models on Azure

Commit all the code on GitHub

Go to portal.azure.com, create an account (I'm using free one), give your account details and Rs. 2 will be deducted

Select create a resource, select web app. <br>
Subscription: Free trial <br>
Resource group: any name <br>
Name: <your-website-name>.azurewebsites.net <br>
Publish: Code/Docker Container
Runtime Stack: the version of your language or framework
OS: Windows
Region: us-east-2 (for Salk AI)
SKU and Size: Free F1

Click on Review + Create (Will take some time)
CLick create
Go to tags and click on Review Plus create and it will get created, will take some (5-6 min) time saying deployment is underway

After deployment is complete, click on go to resources
Select deployment center
Source control: Github
Build provider: App service build service
Configure:
  Organization: Github username
  Repository: <your-github-repo>
  Branch: Master
Then click continue, the finish and deployment will start (will take 5-10 mins, slower than AWS, GCloud)

Then click on your deployment, you can toggle through various options such as deployment center, app logs, overview
