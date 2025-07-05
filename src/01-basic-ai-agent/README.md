Prerequisites
Azure Resources
Azure subscription
Azure AI Foundry project
Deployed AI model (GPT-4, GPT-3.5-turbo, etc.)

Environment Setup
Python 3.8+
Jupyter Notebook or VS Code
Azure CLI (optional)

Environment Variables
Configure your Azure AI services in the .env file at the project root:

# Navigate to the project root and edit the .env file

cd ../../ # Go to azure-ai-agents-playbook root
Update the .env file with your Azure AI project details:

# Required for all tutorials

PROJECT_ENDPOINT="https://your-foundry-resource.services.ai.azure.com/api/projects/your-project-name"
MODEL_DEPLOYMENT_NAME="your-model-deployment-name"

# For Semantic Kernel scenarios

AZURE_OPENAI_API_KEY="your-azure-openai-api-key"
AZURE_OPENAI_ENDPOINT="https://your-openai-resource.openai.azure.com/"
AZURE_OPENAI_CHAT_DEPLOYMENT_NAME="your-chat-deployment"
AZURE_OPENAI_DEPLOYMENT_NAME="your-deployment-name"
AZURE_OPENAI_API_VERSION="2024-12-01-preview"

# Optional: For advanced scenarios

AZURE_SUBSCRIPTION_ID="your-subscription-id"
Tip: The .env file already exists in the project root with example values - just update it with your details.

Required Packages
Install the packages you need:

pip install azure-ai-agents azure-identity semantic-kernel
