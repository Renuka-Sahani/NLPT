# NLPT
# Project Title:  Question-Answering (QA) system using PubMed Data

## Group Members:

Renuka Jawaharlal Sahani - renukasahani16@gmail.com

Suraj Parag Desai - surajdesai3620@gmail.com

Vishal Mangukiya - Vishal.mangukiya875@gmail.com

Radha Mungara - radha.mungara18@gmail.com

#scroll to the last section for logs

## Table of Contents
- [1. Project Description](#1-project-description)
- [2. Installation](#2-installation)
- [3. Contributing](#3-Contributing)
- [4. Data Sources](#4-Data Sources)
- [5. Methodology](#5-Methodology)
- [6. User Interface](#6-User Interface)
- [7. Evaluation and Results](#7-dEvaluation and Results)
- [8. Git commands cheat sheet for project ](#8-git-commands-cheat-sheet)
- [9. Log of contributors to the Project](#notes-for-repo-contributers)

## Description
This project aims to utilize state-of-the-art NLP Transformer models to analyze and categorize legal documents from the PubMed. By leveraging natural language processing techniques, we enhance the accessibility and understanding of complex legal texts for legal professionals and the general public.

![QA_project photo](https://github.com/Renuka-Sahani/NLPT/assets/95965464/afceb6b0-42f2-44f0-b63d-c345ff1d0b3a)


## Installation

on Instructions
```
git clone https://github.com/Renuka-Sahani/NLPT.git
pip install -r requirements.txt
```

## Contributing
We welcome contributions! 

## Data Sources
- PubMed: Medical documents database.

![image](https://github.com/Renuka-Sahani/NLPT/assets/95965464/ed1b863c-b7de-4854-b24a-56eda1fce2da)

## Methodology
Our workflow integrates data acquisition, pre-processing, Transformer model training, and answer generation for legal queries.

## User Interface
The project features a web interface for easy interaction with the system, allowing users to submit queries and receive processed information.

<img width="1512" alt="Screenshot 2024-03-03 at 21 25 13" src="https://github.com/Renuka-Sahani/NLPT/assets/32381311/a31537c9-77ca-4975-8adc-cdf4b39e73fd">

## Evaluation and Results
We evaluated our models based on accuracy, precision, and recall, achieving significant improvements over traditional methods.

## Future Work
- Expand the dataset to include more legal documents.
- Integrate more languages.

## Credits and Acknowledgments
- Team Members: Renuka Sahani, Radha Mungara, Suraj Desai, Vishal Mangukiya
- Mentor: Dr. Jane Doe

##  git commands cheat sheet
 - please don't directly push to main, create a PR and request review or directly contact another member to review before you push. if unsure please just create a PR and wait after requesting review, (patience is a virtue ;-) ) .
1. git pull origin - update your local with your active branch
2. git pull origin main - update your local branch with the latest updates from main
3. git merge --abort - to cancel your merge incase conflicts occur


##  log contributer - for detailed logs, with timings, please refer to the commits page, but we are trying to keep this readme as updated as possible as well
-------------------------------------------------------------

Data Files Acquired- Radha Mungara and Vishal Mangukiya

Git Repo Creation - Renuka Jawaharlal Sahani

Git Folder Creation - Renuka Jawaharlal Sahani

Github access granted - Renuka Jawharlal Sahani

Done research on different paper - Radha Mungara and Vishal Mangukiya

HuggingFace llama created account and requested for access - Suraj Desai 

Pinecone account creation - Suraj Desai

Folder Creation data,src and models - Renuka Jawaharlal Sahani

Uploaded datasets in data folder - Renuka Jawaharlal Sahani

Project Architecture Diagram - Radha Mungara and Vishal Mangukiya

OpenAI key access - Suraj Desai

Automated PubMed Article Retrieval, Processing, and Information Retrieval System Development(without llm and without langchain)- Renuka Jawaharlal Sahani and Suraj Desai

Query Answering System (we used cosine similarities, again without llm and langchain) Radha Mungara and Vishal Mangukiya

converted txt to vector form(Using TF-IDF vectorizer) vectorized_pubmed_data.csv - Suraj Desai and Renuka Sahani

Done information retrieval using single query and multiple queries(again without llm and without langchain) - Vishal Mangukiya and Radha Mungara

We created Three models where we used LLMs:

1) LLM(data from website).ipynb - We have extracted the data directly from PubMed websites and then after that we have created embeddings(Download the OpenAI Embeddings or Hugging Face Embeddings) and after that we  Converted the Text Chunks into Embeddings and Create a Knowledge Base, then we created LLM wrapper,at last we initialize the Retrieval QA with Source Chain,we used llama model here(meta-llama/Llama-2-7b-chat-hf).  -------- done by Vishal Mangukiya and Radha Mungara

2) LLM(with UI).ipynb - This project leverages Langchain and various Large Language Models to build a chatbot that answers questions, utilizing embeddings and Gradio for an interactive UI. ------ done by Renuka Sahani and Suraj Desai

UI Photos: 

<img width="1512" alt="Screenshot 2024-03-03 at 21 23 48" src="https://github.com/Renuka-Sahani/NLPT/assets/32381311/433a20f7-88b5-4494-a061-7b448dc6a3c6">

<img width="1512" alt="Screenshot 2024-03-03 at 21 24 19" src="https://github.com/Renuka-Sahani/NLPT/assets/32381311/18ece928-6b42-4613-8f87-13a89973083f">

3) QA_System_OpenAI.ipynb - We downloaded the data with the necessay filter from the PubMed webiste and stored them in a google drive. Then after we retrieve the files by mounting google drives with the colab notebook.Then we split the data into chunks there after we create function for storing and loading the embeddings.Now we use the OpenAI embeddings to create the vectors and then we initiate the chain to answer question. We then enetered the question and answers them. ------ done by Suraj Desai and Renuka Sahani
