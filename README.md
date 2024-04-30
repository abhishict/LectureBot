## MultiDoc Chatbot

### Description
This project aims to create a chatbot capable of answering questions based on uploaded documents. The chatbot utilizes Natural Language Processing (NLP) techniques to understand user queries and provide relevant responses. 

Implemented this chatbot using the llama-2-70b language model. Here's an explanation of its purpose and the techstack used:
Purpose: The purpose of this code is to create a chatbot that can interact with users in a conversational manner. Users can ask questions about class lectures, and the chatbot will provide responses based on its understanding of the input.


ConversationalRetrievalChain: This is the main component of the chatbot. It manages the conversation flow, retrieves relevant information from the document corpus, and generates responses to user queries.
HuggingFaceEmbeddings: This model is used to embed the text data into vector representations that can be understood by the conversational models.
Replicate (llama-2-70b): This is the conversational language model used by the chatbot. It is responsible for understanding user queries, generating responses, and maintaining context within the conversation.
CharacterTextSplitter: This component splits the input text into smaller chunks for processing, as required by the underlying models.
FAISS: This is the vector store used to index and search the document corpus efficiently.
Overall, this code sets up the necessary components to create a chatbot that can effectively respond to user queries about class lectures using the llama-2-70b language model.

![image](https://github.com/abhishict/LectureBot/assets/28643880/ca7c2457-ca72-4440-9012-434308894588)


### Setup Instructions
1. Create a new virtual environment.
2. Install dependencies listed in the `requirements.txt` file.
3. Sign up on the Replicate portal and obtain an API token.
4. Set up the API token as an environment variable and save it in `.env` file

### Usage
1. Run the `chatapp.py` file using the command `streamlit run chatapp.py`.
2. Upload documents using the file uploader widget.
3. Ask questions related to the uploaded documents using the text input field.
4. The chatbot will generate responses based on the uploaded documents and user queries.

### Code Explanation
- The provided code initializes a Streamlit application.
- It sets up a sidebar for document processing and a file uploader widget to upload documents.
- Uploaded documents are processed, and their text content is extracted.
- The text content is split into smaller chunks for efficient processing.
- Embeddings are created using the Hugging Face embeddings model.
- A vector store is created using FAISS to index the text chunks.
- A conversational chain object is created to handle user queries and provide responses.
- The main function orchestrates the application flow and interaction with the chatbot.

### Running the Application
- To run the application, execute the command `streamlit run chatapp.py` in the terminal.
- Access the application through the provided URL in the terminal.

### Future Improvements
- Integration of multi-modal learning techniques to understand images alongside text.
- Video segmentation and analysis to enhance the chatbot's capabilities.
- Continuous refinement and optimization of the chatbot's responses based on user feedback.

### Contributing
Contributions to the project are welcome. Please feel free to open issues or pull requests on the GitHub repository.

<img width="1504" alt="Screenshot 2024-04-22 at 2 02 12 AM" src="https://github.com/abhishict/LectureBot/assets/28643880/738ba054-d31a-4417-9b07-948d09a5fe32">


