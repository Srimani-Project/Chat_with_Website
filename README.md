# Building a Custom Chatbot from Your Website Data using OpenAI and Langchain

## Introduction:
The goal of this project is to implement a Retrieval-Augmented Generation (RAG) pipeline that allows users to interact with data extracted from websites using advanced natural language processing (NLP) techniques. This system enables users to query a website's content, retrieve relevant information, and generate accurate, context-aware responses by leveraging a large language model (LLM).
## Key Concepts
1. **Retrieval-Augmented Generation (RAG)**:

- A method that combines searching for relevant information (retrieval) with generating responses using AI (generation). The AI uses both the information it retrieves and its own knowledge to answer questions.
2. **Web Scraping**:

- Extracting text and information from websites. The system automatically reads and gathers content like articles, product details, etc.
3. **Text Chunking**:

- Breaking large text into smaller, manageable pieces to make it easier to work with and retrieve specific information.
4. **Vector Embeddings** :

- Converting text into numerical values (vectors) so the system can understand and compare different pieces of information. This helps in finding similar content quickly.
5. **Vector Database**:

- A storage system that holds these vectors, allowing the system to search and retrieve relevant information based on similarity to the user’s query.
6. **Large Language Model (LLM)**:

- AI that understands and generates human-like text. It helps turn the retrieved information into clear, detailed answers.

## How the Application Works:
1. **Data Collection**:

- The system scrapes data from websites (like text, images, and metadata) to gather content.
2. **Data Chunking**:

- The collected text is divided into smaller sections or chunks so it can be processed more easily.
3. **Vector Embedding Creation**:

- Each chunk of text is turned into vectors (numbers), which represent the meaning of the text. This makes it easier to compare and search for relevant information.
4. **Storing in a Database**:

- The vectors, along with their metadata (like the page title), are stored in a vector database.
5. **Query Handling**:

- When a user asks a question, the system turns the question into a vector and searches the database for the most relevant pieces of information.
6. **Generating a Response**:

- The AI takes the retrieved information and generates a detailed, context-rich response, which is given to the user.
7. **User Interaction**:

-The user can continue asking questions, and the system uses the conversation history to provide even better answers.

## Setup Instructions

Follow these steps to set up the project on your local machine:

1. **Clone the Repository:**
   ```
   git clone https://github.com/Srimani-Project/Chat_with_Website.git
   ```

2. **Create a Virtual Environment:**

   Note: We used Python 3.10.11 to create the virtual environment. Please ensure that you use the same Python version to avoid potential conflicts and ensure compatibility with the project dependencies.
   ```
   python3 -m venv venv
   ```

4. **Activate the Virtual Environment:**
   ```
   . venv/bin/activate
   ```

5. **Install Requirements:**
   ```
   pip install -r requirements.txt
   ```

6. **Configure Environment Variables:**
   - Rename `env_sample.sh` to `env.sh`.
   - Add your OpenAI API key to `env.sh`:
     ```
     export OPENAI_API_KEY="your_openai_api_key_here"
     ```

## Usage

Once the project is set up, you can proceed to run the demo code provided in `demo.ipynb` to see the chatbot in action.



