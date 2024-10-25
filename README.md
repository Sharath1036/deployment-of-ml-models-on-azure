# Deployment of ML models on Azure

Commit all the code on GitHub

Go to portal.azure.com, create an account (I'm using free one), give your account details and Rs. 2 will be deducted

Select create a resource, select web app. <br>
Subscription: Free trial <br>
Resource group: any name <br>
Name: &lt;<your-website-name>&gt;.azurewebsites.net <br>
Publish: Code/Docker Container<br>
Runtime Stack: the version of your language or framework<br>
OS: Windows<br>
Region: us-east-2 (for Salk AI)<br>
SKU and Size: Free F1<br>

Click on Review + Create (Will take some time)<br>
CLick create<br>
Go to tags and click on Review Plus create and it will get created, will take some (5-6 min) time saying deployment is underway<br>

After deployment is complete, click on go to resources<br>
Select deployment center<br>
Source control: Github<br>
Build provider: App service build service<br>
Configure:<br>
  Organization: Github username<br>
  Repository: <your-github-repo><br>
  Branch: Master<br>
Then click continue, the finish and deployment will start (will take 5-10 mins, slower than AWS, GCloud)

Then click on your deployment, you can toggle through various options such as deployment center, app logs, overview
