
# Azure OpenAI Hiking Recommendation App

This repository contains a sample application that demonstrates how to integrate Azure OpenAI into a C# or Python application to provide hiking recommendations. The application utilizes the Azure OpenAI Service to interact with a generative AI model, allowing users to ask for hiking suggestions based on their preferences.

## Table of Contents
1. [Prerequisites](#prerequisites)
2. [Getting Started](#getting-started)
3. [Provisioning Azure OpenAI Resource](#provisioning-azure-openai-resource)
4. [Deploying a Model](#deploying-a-model)
5. [Setting Up the Development Environment](#setting-up-the-development-environment)
6. [Configuring the Application](#configuring-the-application)
7. [Adding Code to Use Azure OpenAI](#adding-code-to-use-azure-openai)
8. [Testing the Application](#testing-the-application)
9. [Maintaining Conversation History](#maintaining-conversation-history)
10. [Cleaning Up](#cleaning-up)
11. [Contributing](#contributing)
12. [License](#license)

## Prerequisites
- An Azure subscription with access to Azure OpenAI.
- Visual Studio Code installed on your machine.
- Basic knowledge of C# or Python programming.

## Getting Started
This guide will walk you through the steps to set up and run the Azure OpenAI Hiking Recommendation App.

### 1. Provisioning Azure OpenAI Resource
1. Sign in to the Azure portal at [https://portal.azure.com](https://portal.azure.com).
2. Create an Azure OpenAI resource with the following settings:
   - **Subscription**: Select your approved Azure subscription.
   - **Resource Group**: Create or select `ResourceGroup1lod45818387`.
   - **Region**: Choose any available region (e.g., East US, Japan East).
   - **Name**: Choose a unique name for your resource.
   - **Pricing Tier**: Standard S0.
3. Wait for the deployment to complete.

### 2. Deploying a Model
1. Navigate to your Azure OpenAI resource in the Azure portal.
2. Click on the **Get Started** section to access Azure AI Studio.
3. Create a new deployment of the `gpt-35-turbo-16k` model with the following settings:
   - **Deployment Name**: A unique name of your choice.
   - **Model**: `gpt-35-turbo-16k` (or `gpt-35-turbo` if `16k` is unavailable).
   - **Tokens per minute rate limit**: 5K.
   - **Content filter**: Default.
   - **Enable dynamic quota**: Disabled.

### 3. Setting Up the Development Environment
1. Open Visual Studio Code.
2. Clone the repository:
   ```bash
   git clone https://github.com/MicrosoftLearning/mslearn-openai
Open the cloned folder in Visual Studio Code.
4. Configuring the Application
Navigate to the Labfiles/02-azure-openai-api folder.

Open the folder for your preferred language (C# or Python).

Install the Azure OpenAI SDK package:

For C#:
bash

Verify

Open In Editor
Edit
Copy code
dotnet add package Azure.AI.OpenAI --version 1.0.0-beta.14
For Python:
bash

Verify

Open In Editor
Edit
Copy code
pip install openai==1.13.3
Update the configuration file:

For C#: appsettings.json
For Python: .env
Include your Azure OpenAI resource's endpoint, key, and deployment name.
5. Adding Code to Use Azure OpenAI
Open the main code file:
For C#: Program.cs
For Python: test-openai-model.py
Initialize the Azure OpenAI client and define the system message.
Add code to send requests to the Azure OpenAI model.
6. Testing the Application
Run the application:
For C#: dotnet run
For Python: python test-openai-model.py
Test the application with prompts like:
"What hike should I do near Rainier?"
"Where should I hike near Boise?"
7. Maintaining Conversation History
To enhance the user experience, modify the application to maintain conversation history. This allows the model to reference previous messages and provide more contextual responses.

8. Cleaning Up
After testing, remember to delete the Azure OpenAI resource to avoid incurring charges. Go to the Azure portal and remove the




Share
New
Con
