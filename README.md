# SynGPT

## 🛠️ Built With

[![Python 3.8](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
[![Flask](https://img.shields.io/badge/flask-2.3.2-orange.svg)](https://flask.palletsprojects.com/en/2.1.x/)
[![Node.js](https://img.shields.io/badge/node.js-18.17.1-green.svg)](https://nodejs.org/)
[![React](https://img.shields.io/badge/react-18.2.0-red.svg)](https://reactjs.org/)
[![OpenAI-GPT-3.5](https://img.shields.io/badge/openAI-0.27.8-yellow.svg)](https://openai.com/)

SynGPT is a Python-based application that allows users to read PDFs or uploaded text documents and then ask questions regarding the content of the PDF or text. It utilizes Natural Language Processing (NLP) techniques to understand and answer user questions based on the provided document.

## ✨ Features

- Efficient Document Summarization.
- Accurate Query Responses.
- Easy Document Understanding.
- Quick Doubt Clarification.
- Time saving.

## ⚙️ Pre-requisite
Before running SynChatPDF, make sure you have the following prerequisites installed:

- Docker Install
      [Windows](https://docs.docker.com/desktop/install/windows-install/)
      [Linux](https://docs.docker.com/desktop/install/linux-install/)
      [MAC](https://docs.docker.com/desktop/install/mac-install/)

### Installation

1. Clone the SynGPT repository:

   ```shell
   git clone https://github.com/bhanujoshi24/SynGPT.git
   ```

2. Navigate to the project directory:

   ```shell
   cd SynGPT
   ```
### Docker Setup

3. Build the Docker image:

   ```shell
   docker-compose build 
   ```

4. Run the Docker container:

   ```shell
   docker-compose up
   ```

   This will start the SynGPT backend API in a Docker container.

### Accessing the Frontend

5. Open your web browser and go to:

   [https://bhanujoshi24.github.io/synchatpdf/#/](https://bhanujoshi24.github.io/synchatpdf/#/)

   You can now access the SynGPT frontend and interact with the application.

### Demo Flowchart
[Flowchart](https://spextranet-my.sharepoint.com/personal/sahil_chawla_synpulse_com/_layouts/15/embed.aspx?UniqueId=8035a2c2-9ac3-44a7-8c4e-4cf1ad251fc5&embed=%7B%22ust%22%3Atrue%2C%22hv%22%3A%22CopyEmbedCode%22%7D&referrer=StreamWebApp&referrerScenario=EmbedDialog.Create)

# 🚀 API Details
You can use SynGPT in various ways. Here are some example use cases:

### 📝 Register

**Request**
| Name        | Description                    |
| ----------- | ------------------------------ |
| Username      | text         |
| Password      | text         |
| Email      | text         |

**Response**
| Code        | Description                    |
| ----------- | ------------------------------ |
| 200 OK | If the username is unique, password & email is given properly then the user is created, and a successful register message is returned as a JSON response.|

**Example:** 
```shell
{
    "message": "Registration successful.🎉"
}
```

### 🔑 Login

**Request**
| Name        | Description                    |
| ----------- | ------------------------------ |
| Username      | text         |
| Password      | text         |

**Response**
| Code        | Description                    |
| ----------- | ------------------------------ |
| 200 OK | If the provided credentials match, and a successful login message is returned as a JSON response.|

**Example:** 
```shell
{
    "message": "Login successful!🚀",
    "session_id": "admin_aab69bbd-10d9-41c0-ace3-32def3a89219"
}
```

### 📂 Upload

**Request**
| Name        | Description                    |
| ----------- | ------------------------------ |
| File      | PDF         |

**Response**
| Code        | Description                    |
| ----------- | ------------------------------ |
| 200 OK | It could be a JSON response, a status code, or any other data relevant to the client's request.|

**Example:** 
```shell
[
    {
        "status": "success",
        "text": "Adobe Acrobat PDF Files\nAdobe® Portable Document Format (PDF) is a universal file format that preserves all\nof the fonts, formatting, colours and graphics of any source document, regardless ofthe application and platform used to create it."
    }
]
```

### 📝 User_text

**Request**
| Name        | Description                    |
| ----------- | ------------------------------ |
| Text      | text         |

**Response**
| Code        | Description                    |
| ----------- | ------------------------------ |
| 200 OK | It could be a JSON response, a status code and text.|

**Example:** 
```shell
{
    "status": "success",
    "text": "random access memory"
}
```

### 🔄 Process

**Request**
| Name        | Description                    |
| ----------- | ------------------------------ |
| No data      | No data         |

**Response**
| Code        | Description                    |
| ----------- | ------------------------------ |
| 200 OK | If the processing is successful, the route returns a JSON response with a "status" key set to "success".|

**Example:** 
```shell
{
  "status": "success"
}
```

### 📚 Summary

**Request**
| Name        | Description                    |
| ----------- | ------------------------------ |
| No data      | No data         |

**Response**
| Code        | Description                    |
| ----------- | ------------------------------ |
| 200 OK | If the response status code  is 200 (indicating success), the code proceeds to give summarize text of the whole PDF.|

**Example:** 
```shell
{
    "answer": "The uploaded and processed PDF file is named \"pdf-sample.pdf\" and it is in the Adobe Acrobat PDF format. Adobe PDF is a universal file format that preserves all the fonts, formatting, colors, and graphics of the source document, regardless of the application and platform used to create it.\n\nOne of the key advantages of PDF files is that anyone, anywhere can open them.",
    "question": "Get summary of the uploaded and processed pdf in 200 words.📄"
}
```

### 🙋‍♂️💬 Prompt

**Request**
| Name        | Description                    |
| ----------- | ------------------------------ |
| Prompt(Query)      | text         |

**Response**
| Code        | Description                    |
| ----------- | ------------------------------ |
| 200 OK | The user receives the answer of the input query as a result.|

**Example:** 
```shell
{
  "question": "what's the file type?",
  "answer": "Pdf"
}
```

### 🚪 Logout

**Request**
| Name        | Description                    |
| ----------- | ------------------------------ |
| No data      | No data         |

**Response**
| Code        | Description                    |
| ----------- | ------------------------------ |
| 200 OK | When a request is made to this route, it clears the user's session and returns a message indicating successful logout as a JSON response.|

**Example:** 
```shell
{
    "message": "Logged out successfully.🚪"
}
```

## 📊 Flowchart of SynGPT
![Flowchart](https://github.com/SahilKchawla/syn2/blob/main/Readme%20syn2.png)

## 🚀 Usage

1. Open a web browser and go to `[http://localhost:5000](http://localhost:3000/home)` to access the SynChatPDF web interface.

2. Upload a PDF document or text file by clicking the "Upload" button.

3. Once the document is uploaded, you can start asking questions in the provided input field.

4. SynChatPDF will process your question using NLP techniques and provide answers based on the content of the document.

# 🎥 Video Link
[Video](https://spextranet-my.sharepoint.com/personal/sahil_chawla_synpulse_com/_layouts/15/embed.aspx?UniqueId=95512051-eadf-49b4-8d22-28c38d68b73c&embed=%7B%22ust%22%3Atrue%2C%22hv%22%3A%22CopyEmbedCode%22%7D&referrer=StreamWebApp&referrerScenario=EmbedDialog.Create)
