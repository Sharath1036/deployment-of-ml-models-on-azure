# Deploying Machine Learning Models on Azure

This guide outlines the step-by-step process to deploy your ML models on Azure using a free account.

---

## Prerequisites

1. Code committed to a GitHub repository.
2. An active Azure account (free trial can be used).

---

## Steps for Deployment

### 1. Create an Azure Account
- Go to [portal.azure.com](https://portal.azure.com).
- Create an account. A nominal amount of ₹2 will be deducted for account verification.

---

### 2. Create a Web App
1. **Navigate to:**  
   - Click **Create a resource** > **Web App**.
   
2. **Fill the required fields:**
   - **Subscription:** Free trial  
   - **Resource group:** Any name of your choice  
   - **Name:** `<your-website-name>.azurewebsites.net`  
   - **Publish:** Code/Docker Container  
   - **Runtime Stack:** Choose the version of your language/framework  
   - **OS:** Windows  
   - **Region:** Select a suitable region, e.g., `US East 2`  
   - **SKU and Size:** Free F1  

3. **Complete the creation:**
   - Click **Review + Create** and then **Create**.  
   - This will take **5–6 minutes** to complete the deployment.

4. **Post Deployment:**
   - After deployment, click **Go to resource**.

---

### 3. Configure Deployment Center
1. **Open Deployment Center:**
   - In the resource overview, navigate to **Deployment Center**.

2. **Configure source control:**
   - **Source control:** GitHub  
   - **Build provider:** App Service Build Service  
   - **Configure details:**  
     - **Organization:** Your GitHub username  
     - **Repository:** Select your GitHub repository  
     - **Branch:** Main (or the branch you want to deploy)  

3. **Finalize the setup:**
   - Click **Continue**, then **Finish**. Deployment will start.  
   - The deployment process may take **5–10 minutes**.

---

### 4. Access and Manage the Web App
- After deployment:
  - Access the deployed web app by visiting the URL `<your-website-name>.azurewebsites.net`.
  - Toggle through various options in the Azure portal:
    - **Deployment Center**
    - **App Logs**
    - **Overview**

---

## Notes
- Azure deployments may take longer compared to AWS or GCP.
- Ensure that all dependencies for your ML model are correctly listed in your project configuration (e.g., `requirements.txt` for Python projects).
