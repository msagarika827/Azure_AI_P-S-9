
# Integrate Azure OpenAI into your app

This repository contains a sample application that demonstrates how to integrate Azure OpenAI into a Python application to provide hiking recommendations. The application utilizes the Azure OpenAI Service to interact with a generative AI model, allowing users to ask for hiking suggestions based on their preferences.

## Table of Contents
1. [Prerequisites]
2. [Getting Started]
3. [Provisioning Azure OpenAI Resource]
4. [Deploying a Model]
5. [Setting Up the Development Environment]
6. [Configuring the Application]
7. [Adding Code to Use Azure OpenAI]
8. [Testing the Application]
9. [Maintaining Conversation History]
10. [Cleaning Up]
11. [Contributing]
12. [License]

## Prerequisites
- An Azure subscription with access to Azure OpenAI.
- Visual Studio Code installed on your machine.
- Basic knowledge of C# or Python programming.

## Getting Started
This guide will walk you through the steps to set up and run the Azure OpenAI Hiking Recommendation App.

### 1. Provisioning Azure OpenAI Resource
1. Sign in to the Azure portal at [https://portal.azure.com](https://portal.azure.com).
2. Create an Azure OpenAI resource with the following settings:
   - **Subscription**: 
   - **Resource Group**: 
   - **Region**:
   - **Name**: 
   - **Pricing Tier**:
3. Wait for the deployment to complete.

### 2. Deploying a Model
1. Navigate to your Azure OpenAI resource in the Azure portal.
2. Click on the **Get Started** section to access Azure AI Studio.
3. Create a new deployment of the `gpt-35-turbo-16k` model with the following settings:
   - **Deployment Name**: 
   - **Model**: 
   - **Tokens per minute rate limit**: 
   - **Content filter**: 
   - **Enable dynamic quota**: 

### 3. Setting Up the Development Environment
1. Open Visual Studio Code.
2. Clone the repository:
   ```bash
   git clone https://github.com/MicrosoftLearning/mslearn-openai
Open the cloned folder in Visual Studio Code.
4. Configuring the Application

pip install openai==1.13.3

For Python: .env
Include your Azure OpenAI resource's endpoint, key, and deployment name.
5. Adding Code to Use Azure OpenAI
Open the main code file:

For Python: test-openai-model.py
Initialize the Azure OpenAI client and define the system message.

6. Testing the Application
Run the application:

For Python: python test-openai-model.py
Test the application with prompts like:
"What hike should I do near Rainier?"
"Where should I hike near Boise?"
