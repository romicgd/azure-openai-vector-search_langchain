# Using OpenAI and langchain with Azure Cognitive Search Vector Search and Azure Form Recognizer

This project demonstrates how to use langchain and OpenAI with your own data. The goal is to show how to use these technologies together to build a search engine that can find relevant information in your own data.
Also this project compares the use of different OpenAI models to provide answer to the same question: ```gpt-4``` and ```text-davinci-003```.

## Prerequisites

Before you begin, you'll need to have the following:

- An Azure account with access to Azure Cognitive Search and Azure Form Recognizer
- A dataset of documents that you want to search through
- An OpenAI API key

.env needs to contain following 
(separate endpoints for ```gpt-4``` and ```text-davinci-003``` models as currently different subset of OpenAI models are available in different Azure regions)
```
   AZURE_SEARCH_SERVICE=...
   AZURE_SEARCH_INDEX_NAME=...
   AZURE_SEARCH_ADMIN_KEY=...
   CHATGPT_OPENAI_API_BASE=https://%%%%%.openai.azure.com/
   CHATGPT_OPENAI_API_KEY=...
   DAVINCI_OPENAI_API_BASE=https://%%%%%.openai.azure.com/
   DAVINCI_OPENAI_API_KEY=...
   OPENAI_API_VERSION=2023-05-15
   AZURE_FORMRECOGNIZER_KEY=...
   AZURE_FORMRECOGNIZER_SERVICE=...
   AZURESEARCH_FIELDS_CONTENT_VECTOR=contentVector
```