# Student REST API 

This is a RESTful API for managing student records, allowing CRUD operations (Create, Read, Update, Delete) for a Student entity.

## Features

- Retrieve a list of all students.
- Retrieve details of a student by ID
- Add a new student
- Update an existing student by ID
- Delete a student by ID

## Prerequisites

Before you can run or deploy this app, you need to have the following installed:

- ### Prerequisites
- Python 3.x
- Flask and SQLAlchemy
- Azure CLI (optional, for deployment)

## Project Structure

- app.py: Main Flask application 
- requirements.txt: List of Python dependencies 
- test-api.http: Test the REST API using the REST Client extension in Visual Studio Code
- README.md: Documentation

## Running Locally

To run the Flask API on your local machine:

1. Clone this repository:

   ```bash
   git clone https://github.com/bhupinder2414/Rest API.git
   
2. Navigate to the project directory:
   ```bash
   cd Rest API

3. Set up a Virtual envirnoment
```bash
python3 -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
```
3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   
4. Run the application:
   ```bash
   python3 app.py
5. The API will be running at http://127.0.0.1:5000/
6. Use **test-api.http** to test the REST API using the REST Client extension in Visual Studio Code.

## Deploying to Azure

### What is Azure App Service?

[Azure App Service](https://learn.microsoft.com/en-us/azure/app-service/) is a fully managed platform for building, deploying, and scaling web apps. With Azure App Service, you can host web applications, REST APIs, and mobile backends in any programming language without managing infrastructure. It provides integrated continuous deployment and scaling features, making it a powerful and flexible solution for cloud-based web hosting.

### Step 6: Deploy to Azure
1. **Create an Azure Web App**:
   - Go to Azure Portal, create a new Web App, and choose Python as the runtime stack.

2. **Deploy**:
   - Use the [Azure CLI](https://learn.microsoft.com/en-us/azure/app-service/quickstart-python) to deploy or set up GitHub Actions for continuous deployment.

Some key features of Azure App Service include:
- **Automatic Scaling**: Scale up or out depending on traffic.
- **Continuous Integration/Continuous Deployment (CI/CD)**: Easily integrate with GitHub, Bitbucket, or Azure DevOps for automated deployments.
- **Custom Domains and SSL**: Secure your apps with custom domains and certificates.
- **Load Balancing**: Built-in load balancing to handle high-traffic applications.
- **Monitoring and Diagnostics**: Access real-time monitoring and logs for troubleshooting.


You can learn more about Azure App Service and its features in the [official documentation](https://learn.microsoft.com/en-us/azure/app-service/).

To learn how to deploy a Python web app (Django, Flask, or FastAPI) to Azure App Service, refer to the [Quickstart Guide](https://learn.microsoft.com/en-us/azure/app-service/quickstart-python?tabs=flask%2Cwindows%2Cazure-cli%2Cazure-cli-deploy%2Cdeploy-instructions-azportal%2Cterminal-bash%2Cdeploy-instructions-zip-azcli). This guide walks you through deploying a Python web app to Azure, leveraging App Service to run your app in a Linux server environment.

