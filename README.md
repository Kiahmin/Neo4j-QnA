# Neo4j-QnA Chatbot

## Overview

This repository contains a QnA chatbot that connects to a movie database in Neo4j. The chatbot can answer questions about movies, including their release dates, taglines, and directors. The project leverages the neo4j-driver to interact with the Neo4j database, spaCy for natural language processing, and Gradio for the user interface.

## Features

- Extracts entities from user queries using SpaCy.
- Connects to a Neo4j database to fetch information about movies.
- Answers questions about movie release dates, taglines, and directors.
- Interactive user interface built with Gradio.

## Installation

To get started with Neo4j-QnA, you need to have Python installed on your machine. Follow the steps below to set up the project:

1. **Clone the repository:**

   ```sh
   git clone https://github.com/your-username/Neo4j-QnA.git
   cd Neo4j-QnA

2. **Install Neo4j Driver:**
   ```sh
   npm install --save neo4j-driver
   
3. **Change driver connection details**
   Open the chatbot.ipynb file and change the driver connection details to your own. You may find the connection details of your neo4j project here:
![image](https://github.com/user-attachments/assets/30b766c4-b7f7-42a5-ad9b-49d6882c1e74)

   Credentials used in this code will expire so remember to use your own.

4. **Run the notebook:**
After changing driver connection details, run all cells. This will install all necessary packages, download the SpaCy model, and start the chatbot application.

## Usage
After running the application, you can interact with the chatbot through the Gradio interface. You can ask questions like:

- When was the movie "RescueDawn" released?
- What is the tagline of the movie "RescueDawn"?
- Who is the director of the movie "RescueDawn"?

The chatbot will extract relevant entities from your questions and query the Neo4j database to provide the answers.

## Dependancies
- neo4j-driver: Python driver for connecting to the Neo4j database.
- spacy: NLP library for extracting entities from user queries.
- gradio: Library for creating an interactive user interface.
