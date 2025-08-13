Cold Email Generator

A smart application that streamlines the job application process by generating personalized cold emails to HR. 
This tool web scrapes job descriptions from a given URL and uses a Large Language Model LLM to craft a compelling customized email all within a user-friendly Streamlit interface.

Features
Web Scraping Automatically extracts key information from job descriptions using a provided URL.
AI-Powered Email Generation Leverages a powerful LLM to write a targeted cold email based on the scraped job details.
Customization The generated email can be further edited and tailored to your specific needs before being sent.
Intuitive UI Built with Streamlit for a simple and elegant user experience.

Technologies Used
Python The core programming language for the application.
Streamlit For creating the interactive and user-friendly web interface.
LangChain The framework used to build the LLM application.
langchain==0.2.14
langchain-community==0.2.12
langchain-groq===0.1.9
Vector Database
chromadb==0.5.0 Used as the vector store for managing and retrieving text embeddings.
Web Scraping
selenium==4.21.0 For navigating and extracting data from web pages.
unstructured==0.14.6 To process and parse the unstructured data from the web pages.
Data Handling
pandas==2.0.2 For data manipulation and analysis if needed.
Environment Management
python-dotenv==1.0.0 To securely manage environment variables.

How to Run Locally

1.  Clone the repository
    git clone [https://github.com/Maddi-Jagadeesh/cold-email-generator.git]
    cd cold-email-generator
2.  Set up a virtual environment
    python -m venv venv
    source venv/bin/activate On Windows use venv\\Scripts\\activate
3.  Install the dependencies
    pip install -r requirements.txt
    Ensure you have a requirements.txt file listing all the libraries.
4.  Configure API Keys
    Create a .env file in the root directory and add your API key for the LLM.
    GROQ\_API\_KEY=your\_groq\_api\_key\_here
5.  Run the Streamlit application
    streamlit run your\_app\_file\_name.py
    This will open the application in your web browser.
