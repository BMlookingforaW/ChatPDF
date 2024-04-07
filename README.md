# PDF Question Answering Web Application

Welcome to our PDF Question Answering Web Application! This application allows users to ask questions related to PDF documents uploaded by them. We utilize the Gemini conversational AI model to generate answers based on the content of the PDF files.

## Architecture

![image](https://github.com/BMlookingforaW/ChatPDF/assets/99363954/05b15e67-951d-481f-a068-ddf8fb11154b)

### User Interaction
- Users can interact with the web application through a simple and intuitive user interface.
- They can ask questions using a text input field and upload PDF files for processing.

### Backend Processing
- The backend processing involves the following steps:
  1. **Extract Text**: Text is extracted from the uploaded PDF files using PyPDF2.
  2. **Text Chunking**: The extracted text is split into smaller chunks for efficient processing.
  3. **Vector Store Creation**: We create a vector store based on the text chunks using Google Generative AI Embeddings and FAISS.
  4. **Conversational Chain Configuration**: We configure a conversational chain for question-answering using the Gemini conversational AI model.
  5. **Answer Generation**: The system generates an answer based on the user's question and the context from the vector store.

### Response Display
- The generated answer is displayed back to the user through the web interface, providing them with the information they need.

## Restrictions
To ensure smooth operation and compliance with usage limits, we have the following restrictions:
- **2 RPM (requests per minute)**
- **32,000 TPM (tokens per minute)**
- **50 RPD (requests per day)**

## How to Use
1. Navigate to our web application.
2. Ask a question related to the uploaded PDF files.
3. Upload your PDF files using the provided file uploader.
4. Click the "Submit & Process" button to initiate processing.
5. Wait for the system to generate an answer based on your question and the content of the PDF files.
6. View the generated answer displayed on the screen.

