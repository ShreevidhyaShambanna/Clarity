EmpathAI - AI for Mental Wellness

Overview
EmpathAI is a chatbot designed to assist users by providing support and information on common mental health issues. It leverages natural language processing (NLP) and machine learning (ML) to interact with users in a conversational manner, understanding their concerns and offering appropriate guidance or resources.

Data Sources
The project utilizes multiple MentalHealthChat Datasets from Hugging Face for training the chatbot.

Setup and Installation
To get started with EmpathAI, follow these steps to set up your environment.

Prerequisites
Python 3.10
pip
virtualenv or conda (optional, but recommended for creating an isolated environment)

Installing Dependencies: Clone the repository and navigate to the project directory:

git clone <repository-url>
cd empathai

Install the required dependencies:

pip install -r requirements/requirements.txt

Data
Due to the large size of the data, it's not tracked by Git. After cloning the repository, download and place the datasets in the appropriate directory as specified in the data loading scripts.

We gathered datasets from these sources:
https://huggingface.co/datasets/hizardev/MentalHealthChat
https://huggingface.co/datasets/Kanakmi/mental-disorders
https://huggingface.co/datasets/Amod/mental_health_counseling_conversations
https://huggingface.co/datasets/heliosbrahma/mental_health_chatbot_dataset
https://huggingface.co/datasets/vibhorag101/phr_mental_therapy_dataset
https://huggingface.co/datasets/jsfactory/mental_health_reddit_posts
https://huggingface.co/datasets/Riyazmk/mentalhealth
https://huggingface.co/datasets/alexandreteles/mental-health-conversational-data
https://huggingface.co/datasets/mpingale/mental-health-chat-dataset


Usage

To run the EmpathAI chatbot, execute the main.py script:
python main.ipnb

Repository Structure
The repository is organized into several key folders:
data/: Scripts related to data loading and preprocessing.
utils/: Utility scripts for embeddings generation, clustering, and data visualization.
models/: Model-related scripts for BERT sequence classification and GPT-3 interactions.
requirements/: Contains requirements.txt and environment.yml for dependency management.
README.md: This file, containing the project overview and instructions.

How It Works - EmpathAI processes input text from the user to determine the intent and generate an appropriate response. The process involves:

1. Preprocessing input data.
2. Generating embeddings for the input text.
3. Clustering the embeddings to classify intents.
4. Utilizing BERT for sequence classification.
5. Generating responses using OpenAI's GPT-3 based on classified intents.

For more detailed information on each step, refer to the corresponding scripts in the data/, utils/, and models/ directories.


Acknowledgments
Hugging Face for providing the datasets.
OpenAI for GPT-3 API access.
