
# Automated Exam Paper checking using Semantic analysis

Semantic analysis is a process of understanding the meaning of text.This repository contains the code to develop an automated exam paper checking system that uses semantic analysis to compare the expected answer and student response to evaluate student responses.




## Installation

use below command to install all required dependencies

```bash
pip install numpy==1.23.4
pip install PyTorch==1.6.0
pip install transformers==4.26.0
pip install sentence-transformers==2.2.2
pip install PyPDF2==3.0.1
```
    
## Usage

- #### Install Dependencies and Libraries
- #### Import Library
- #### Extract text from pdf using PdfReader module from PyPDF2 tool




- #### Model Selection and Initialization
      recomended to use 'stsb-roberta-large', as it is the best model for  the task of semantic similarity.

- #### After extracting text from pdf, split them question wise.
- #### Calculate semantic similarity between student answer and expected answer for the particular question.

- #### For semantic similarity
      1. Use the selected model to encode the sentences which creates sentence level embeddings.
      2. Calculating the cosine similarity between embeddingsof student answer and expected answer.
      3. The final result will be score for the student response.

- **Note:** Refer given Jupyter Notebook for code of Automated Exam Paper checking using semantic analysis with example

## Running Tests

- #### Approach 1
To run tests, use testing files 
```
For student Answers file - 'Sushmita_15.pdf'
For Expected Answers file - 'Science_Answers.pdf'

```


- #### Approach 2

Pass student answer and Expected answer to score() method which will return the score for student response w.r.t Expected answer










## Features

- The system will be capable of handling a wide range of exam questions and response types, including breif-type questions, multiple-choice questions, and short-answer questions.

- The system will provide detailed evaluation with respect to each question and also provides the total score for the student response.


## Tech Stack

**Python:** Numpy, Pandas, Sentence-Transformer, PyTorch

