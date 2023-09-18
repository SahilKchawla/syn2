Sure, here's a more complete README file in Markdown format for the GitHub project "synchatpdf":

# SynGPT

## Built With

[![Python 3.8](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
[![Flask](https://img.shields.io/badge/flask-2.3.2-orange.svg)](https://flask.palletsprojects.com/en/2.1.x/)
[![Node.js](https://img.shields.io/badge/node.js-18.17.1-green.svg)](https://nodejs.org/)
[![React](https://img.shields.io/badge/react-18.2.0-red.svg)](https://reactjs.org/)
[![OpenAI-GPT-3.5](https://img.shields.io/badge/openAI-0.27.8-yellow.svg)](https://openai.com/)

SynGPT is a Python-based application that allows users to read PDFs or uploaded text documents and then ask questions regarding the content of the PDF or text. It utilizes Natural Language Processing (NLP) techniques to understand and answer user questions based on the provided document.

## Features

- Upload PDF documents or text files.
- Ask questions about the content.
- Get answers based on the document's content.
- Easy-to-use web interface.
- Built-in support for common questions and commands.

## Pre-requisite
Before running SynChatPDF, make sure you have the following prerequisites installed:

- Python (version 3.6)
- Backend Code Installed - [https://github.com/bhanujoshi24/SynGPT]

# Use-Cases
You can use SynGPT in various ways. Here are some example use cases:

### Register

**Parameters**
| Name        | Description                    |
| ----------- | ------------------------------ |
| Username      | text         |
| Password      | text         |
| Email      | text         |

**Response**
| Code        | Description                    |
| ----------- | ------------------------------ |
| 200 OK | If the username is unique, password and email is given properly then the user is created, and a successful login message is returned as a JSON response.|

**Example:** 
{
    "message": "Registration successful."
}     
## Flowchart of SynGPT
![Flowchart](https://github.com/SahilKchawla/syn2/blob/main/Readme%20syn2.png)

## Usage

1. Open a web browser and go to `[http://localhost:5000](http://localhost:3000/home)` to access the SynChatPDF web interface.

2. Upload a PDF document or text file by clicking the "Upload" button.

3. Once the document is uploaded, you can start asking questions in the provided input field.

4. SynChatPDF will process your question using NLP techniques and provide answers based on the content of the document.

# Video Link
Video : https://spextranet-my.sharepoint.com/personal/sahil_chawla_synpulse_com/_layouts/15/embed.aspx?UniqueId=95512051-eadf-49b4-8d22-28c38d68b73c&embed=%7B%22ust%22%3Atrue%2C%22hv%22%3A%22CopyEmbedCode%22%7D&referrer=StreamWebApp&referrerScenario=EmbedDialog.Create
