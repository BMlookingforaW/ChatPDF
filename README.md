- Streamlit web application that allows users to ask questions related to PDF documents uploaded by them. It utilizes the Gemini conversational AI model to answer questions based on the content of the PDF files.

- Architecture:-
  ![image](https://github.com/BMlookingforaW/ChatPDF/assets/99363954/05b15e67-951d-481f-a068-ddf8fb11154b)
  - The user interacts with the user interface by asking a question and uploading PDF files.
  - The backend processing involves several steps:
    - Extracting text from the uploaded PDF files.
    - Splitting the text into smaller chunks.
    - Creating a vector store based on the text chunks.
    - Configuring the conversational chain for question-answering.
    - Generating an answer based on the user's question and the context from the vector store.
  - The response is then displayed back to the user through the user interface.

- Restrictions:-
  - 2 RPM (requests per minute)
  - 32,000 TPM (tokens per minute)
  - 50 RPD (requests per day)
