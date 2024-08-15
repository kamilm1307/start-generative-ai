![Generative AI For Beginners](./images/repo-thumbnailv3.png?WT.mc_id=academic-105485-koreyst)

### 18 Lessons teaching everything you need to know to start building Generative AI applications

[![GitHub license](https://img.shields.io/github/license/microsoft/Generative-AI-For-Beginners.svg)](https://github.com/microsoft/Generative-AI-For-Beginners/blob/master/LICENSE?WT.mc_id=academic-105485-koreyst)
[![GitHub contributors](https://img.shields.io/github/contributors/microsoft/Generative-AI-For-Beginners.svg)](https://GitHub.com/microsoft/Generative-AI-For-Beginners/graphs/contributors/?WT.mc_id=academic-105485-koreyst)
[![GitHub issues](https://img.shields.io/github/issues/microsoft/Generative-AI-For-Beginners.svg)](https://GitHub.com/microsoft/Generative-AI-For-Beginners/issues/?WT.mc_id=academic-105485-koreyst)
[![GitHub pull-requests](https://img.shields.io/github/issues-pr/microsoft/Generative-AI-For-Beginners.svg)](https://GitHub.com/microsoft/Generative-AI-For-Beginners/pulls/?WT.mc_id=academic-105485-koreyst)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com?WT.mc_id=academic-105485-koreyst)

[![GitHub watchers](https://img.shields.io/github/watchers/microsoft/Generative-AI-For-Beginners.svg?style=social&label=Watch)](https://GitHub.com/microsoft/Generative-AI-For-Beginners/watchers/?WT.mc_id=academic-105485-koreyst)
[![GitHub forks](https://img.shields.io/github/forks/microsoft/Generative-AI-For-Beginners.svg?style=social&label=Fork)](https://GitHub.com/microsoft/Generative-AI-For-Beginners/network/?WT.mc_id=academic-105485-koreyst)
[![GitHub stars](https://img.shields.io/github/stars/microsoft/Generative-AI-For-Beginners.svg?style=social&label=Star)](https://GitHub.com/microsoft/Generative-AI-For-Beginners/stargazers/?WT.mc_id=academic-105485-koreyst)

[![](https://dcbadge.vercel.app/api/server/ByRwuEEgH4)](https://aka.ms/genai-discord?WT.mc_id=academic-105485-koreyst)

# Generative AI for Beginners (Version 2) - A Course

Learn the fundamentals of building Generative AI applications with our 18-lesson comprehensive course by Microsoft Cloud Advocates.

## 🌱 Getting Started

This course has 18 lessons. Each lesson covers its own topic so start wherever you like!

Lessons are labeled either "Learn" lessons explaining a Generative AI concept or "Build" lessons that explain a concept and code examples in both **Python** and **TypeScript** when possible.

Each lesson also includes a "Keep Learning" section with additional learning tools.

**What You Need**

- Access to the [Azure OpenAI Service](https://azure.microsoft.com/products/ai-services/openai-service?WT.mc_id=academic-105485-koreyst) **OR** [OpenAI API](https://platform.openai.com/docs/quickstart?context=python?WT.mc_id=academic-105485-koreyst) **OR** [GitHub Marketplace Model Catalog](https://github.com/marketplace/models?WT.mc_id=academic-105485-koreyst) - _Only required to complete coding lessons_
- Basic knowledge of Python or TypeScript is helpful - \*For absolute beginners check out these [Python](https://learn.microsoft.com/training/paths/python-language/?WT.mc_id=academic-105485-koreyst) and [TypeScript](https://learn.microsoft.com/training/paths/build-javascript-applications-typescript/?WT.mc_id=academic-105485-koreyst) courses.
- A GitHub account to [fork this entire repo](https://github.com/microsoft/generative-ai-for-beginners/fork?WT.mc_id=academic-105485-koreyst) to your own GitHub account

We have created a **[Course Setup](./00-course-setup/README.md?WT.mc_id=academic-105485-koreyst)** lesson to help you with setting up your development environment.

Don't forget to [star (🌟) this repo](https://docs.github.com/en/get-started/exploring-projects-on-github/saving-repositories-with-stars?WT.mc_id=academic-105485-koreyst) to find it easier later.

## Step-by-step guide to set up an Azure OpenAI free account

### Step 1: Sign Up for an Azure Account
1. **Visit Azure Portal:**
   Go to the [Azure portal](https://azure.microsoft.com/products/ai-services/openai-service?WT.mc_id=academic-105485-koreyst).

2. **Create an Account:**
   If you don't already have an Azure account, click on "Start free" and follow the instructions to create an account. You'll need to provide some personal information and a valid payment method (credit card) for identity verification. Note that while setting up the account is free, some services might incur costs, but you can access many free services with the Azure free account.

### Step 2: Access Azure OpenAI Service
1. **Navigate to Azure OpenAI:**
   Once logged into the Azure portal, search for "Azure OpenAI" in the search bar at the top.

2. **Create an OpenAI Service:**
   Click on "Create" under the Azure OpenAI Service. You will be taken to the "Create OpenAI Service" page.

### Step 3: Configure Your OpenAI Service
1. **Select Subscription:**
   Choose your Azure subscription from the dropdown.

2. **Resource Group:**
   Create a new resource group or select an existing one. A resource group is a container that holds related resources for an Azure solution.

3. **Region:**
   Select a region where you want to host your OpenAI service.

4. **Name Your OpenAI Service:**
   Provide a unique name for your OpenAI service.

5. **Pricing Tier:**
   Select a pricing tier. If you're using a free account, make sure to select a free or trial tier if available.

6. **Review and Create:**
   Click on "Review + create" to review your settings, and then click "Create" to deploy the service.

### Step 4: Obtain the API Key
1. **Navigate to the Resource:**
   Once the deployment is complete, navigate to your OpenAI resource by clicking on "Go to resource".

2. **Access Keys:**
   In the left-hand menu, under "Keys and Endpoint," you will find your API keys.

3. **Copy the Key:**
   Copy the primary key. This is your API key that you will use to authenticate your requests to the Azure OpenAI service.

### Step 5: Use the API Key
1. **Install Azure SDK:**
   Depending on your development environment, you might need to install the Azure SDK. For example, for Python:
   ```bash
   pip install azure-ai-openai
   ```

2. **Authenticate Using the API Key:**
   Use the API key in your application to authenticate and make requests. For example, in Python:
   ```python
   from azure.ai.openai import OpenAIClient
   from azure.core.credentials import AzureKeyCredential

   api_key = 'YOUR_API_KEY'
   endpoint = 'https://YOUR_RESOURCE_NAME.openai.azure.com/'

   client = OpenAIClient(endpoint=endpoint, credential=AzureKeyCredential(api_key))

   # Now you can use the client to interact with the OpenAI service
   ```

### Additional Resources
- **Azure Documentation:** For more detailed information, refer to the Azure OpenAI Service documentation.
- **Support:** If you run into any issues, Azure support is available through the portal.


## 🧠 Ready to Deploy?

If you are looking for more advanced code samples, check out our [collection of Generative AI Code Samples](https://aka.ms/genai-beg-code?WT.mc_id=academic-105485-koreyst) in both **Python** and **TypeScript**.

## 🗣️ Meet Other Learners, Get Support

Join our [official AI Discord server](https://aka.ms/genai-discord?WT.mc_id=academic-105485-koreyst) to meet and network with other learners taking this course and get support.

## 🚀 Building a Startup?

Sign up for [Microsoft for Startups Founders Hub](https://aka.ms/genai-foundershub?WT.mc_id=academic-105485-koreyst) to receive **free OpenAI credits** and up to **$150k towards Azure credits to access OpenAI models through Azure OpenAI Services**.

## 🙏 Want to help?

Do you have suggestions or found spelling or code errors? [Raise an issue](https://github.com/microsoft/generative-ai-for-beginners/issues?WT.mc_id=academic-105485-koreyst) or [Create a pull request](https://github.com/microsoft/generative-ai-for-beginners/pulls?WT.mc_id=academic-105485-koreyst)

## 📂 Each lesson includes:

- A short video introduction to the topic
- A written lesson located in the README
- Python and TypeScript code samples supporting Azure OpenAI and OpenAI API
- Links to extra resources to continue your learning

## 🗃️ Lessons

| #   | **Lesson Link**                                                                                                                              | **Description**                                                                                 | **Video**                                                                   | **Extra Learning**                                                             |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| 00  | [Course Setup](./00-course-setup/README.md?WT.mc_id=academic-105485-koreyst)                                                                 | **Learn:** How to Setup Your Development Environment                                            | Coming Soon                                                                 | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 01  | [Introduction to Generative AI and LLMs](./01-introduction-to-genai/README.md?WT.mc_id=academic-105485-koreyst)                              | **Learn:** Understanding what Generative AI is and how Large Language Models (LLMs) work.       | [Video](https://aka.ms/gen-ai-lesson-1-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 02  | [Exploring and comparing different LLMs](./02-exploring-and-comparing-different-llms/README.md?WT.mc_id=academic-105485-koreyst)             | **Learn:** How to select the right model for your use case                                      | [Video](https://aka.ms/gen-ai-lesson2-gh?WT.mc_id=academic-105485-koreyst)  | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 03  | [Using Generative AI Responsibly](./03-using-generative-ai-responsibly/README.md?WT.mc_id=academic-105485-koreyst)                           | **Learn:** How to build Generative AI Applications responsibly                                  | [Video](https://aka.ms/gen-ai-lesson3-gh?WT.mc_id=academic-105485-koreyst)  | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 04  | [Understanding Prompt Engineering Fundamentals](./04-prompt-engineering-fundamentals/README.md?WT.mc_id=academic-105485-koreyst)             | **Learn:** Hands-on Prompt Engineering Best Practices                                           | [Video](https://aka.ms/gen-ai-lesson4-gh?WT.mc_id=academic-105485-koreyst)  | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 05  | [Creating Advanced Prompts](./05-advanced-prompts/README.md?WT.mc_id=academic-105485-koreyst)                                                | **Learn:** How to apply prompt engineering techniques that improve the outcome of your prompts. | [Video](https://aka.ms/gen-ai-lesson5-gh?WT.mc_id=academic-105485-koreyst)  | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 06  | [Building Text Generation Applications](./06-text-generation-apps/README.md?WT.mc_id=academic-105485-koreyst)                                | **Build:** A text generation app using Azure OpenAI / OpenAI API                                | [Video](https://aka.ms/gen-ai-lesson6-gh?WT.mc_id=academic-105485-koreyst)  | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 07  | [Building Chat Applications](./07-building-chat-applications/README.md?WT.mc_id=academic-105485-koreyst)                                     | **Build:** Techniques for efficiently building and integrating chat applications.               | [Video](https://aka.ms/gen-ai-lessons7-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 08  | [Building Search Apps Vector Databases](./08-building-search-applications/README.md?WT.mc_id=academic-105485-koreyst)                        | **Build:** A search application that uses Embeddings to search for data.                        | [Video](https://aka.ms/gen-ai-lesson8-gh?WT.mc_id=academic-105485-koreyst)  | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 09  | [Building Image Generation Applications](./09-building-image-applications/README.md?WT.mc_id=academic-105485-koreyst)                        | **Build:** A image generation application                                                       | [Video](https://aka.ms/gen-ai-lesson9-gh?WT.mc_id=academic-105485-koreyst)  | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 10  | [Building Low Code AI Applications](./10-building-low-code-ai-applications/README.md?WT.mc_id=academic-105485-koreyst)                       | **Build:** A Generative AI application using Low Code tools                                     | [Video](https://aka.ms/gen-ai-lesson10-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 11  | [Integrating External Applications with Function Calling](./11-integrating-with-function-calling/README.md?WT.mc_id=academic-105485-koreyst) | **Build:** What is function calling and its use cases for applications                          | [Video](https://aka.ms/gen-ai-lesson11-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 12  | [Designing UX for AI Applications](./12-designing-ux-for-ai-applications/README.md?WT.mc_id=academic-105485-koreyst)                         | **Learn:** How to apply UX design principles when developing Generative AI Applications         | [Video](https://aka.ms/gen-ai-lesson12-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 13  | [Securing Your Generative AI Applications](./13-securing-ai-applications/README.md?WT.mc_id=academic-105485-koreyst)                         | **Learn:** The threats and risks to AI systems and methods to secure these systems.             | [Video](https://aka.ms/gen-ai-lesson13-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 14  | [The Generative AI Application Lifecycle](./14-the-generative-ai-application-lifecycle/README.md?WT.mc_id=academic-105485-koreyst)           | **Learn:** The tools and metrics to manage the LLM Lifecycle and LLMOps                         | [Video](https://aka.ms/gen-ai-lesson14-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 15  | [Retrieval Augmented Generation (RAG) and Vector Databases](./15-rag-and-vector-databases/README.md?WT.mc_id=academic-105485-koreyst)        | **Build:** An application using a RAG Framework to retrieve embeddings from a Vector Databases  | [Video](https://aka.ms/gen-ai-lesson15-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 16  | [Open Source Models and Hugging Face](./16-open-source-models/README.md?WT.mc_id=academic-105485-koreyst)                                    | **Build:** An application using open source models available on Hugging Face                    | [Video](https://aka.ms/gen-ai-lesson16-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 17  | [AI Agents](./17-ai-agents/README.md?WT.mc_id=academic-105485-koreyst)                                                                       | **Build:** An application using an AI Agent Framework                                           | [Video](https://aka.ms/gen-ai-lesson17-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |
| 18  | [Fine-Tuning LLMs](./18-fine-tuning/README.md?WT.mc_id=academic-105485-koreyst)                                                              | **Learn:** The what, why and how of fine-tuning LLMs                                            | [Video](https://aka.ms/gen-ai-lesson18-gh?WT.mc_id=academic-105485-koreyst) | [Learn More](https://aka.ms/genai-collection?WT.mc_id=academic-105485-koreyst) |

### 🌟 Special thanks

Special thanks to [**John Aziz**](https://www.linkedin.com/in/john0isaac/) for creating all of the GitHub Actions and workflows

## 🎒 Other Courses

Our team produces other courses! Check out:

- [ML for Beginners](https://aka.ms/ml-beginners?WT.mc_id=academic-105485-koreyst)
- [Data Science for Beginners](https://aka.ms/datascience-beginners?WT.mc_id=academic-105485-koreyst)
- [AI for Beginners](https://aka.ms/ai-beginners?WT.mc_id=academic-105485-koreyst)
- [**NEW** Cybersecurity for Beginners](https://github.com/microsoft/Security-101??WT.mc_id=academic-96948-sayoung)
- [Web Dev for Beginners](https://aka.ms/webdev-beginners?WT.mc_id=academic-105485-koreyst)
- [IoT for Beginners](https://aka.ms/iot-beginners?WT.mc_id=academic-105485-koreyst)
- [XR Development for Beginners](https://github.com/microsoft/xr-development-for-beginners?WT.mc_id=academic-105485-koreyst)
- [Mastering GitHub Copilot for AI Paired Programming](https://aka.ms/GitHubCopilotAI?WT.mc_id=academic-105485-koreyst)
