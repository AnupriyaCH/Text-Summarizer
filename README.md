# Text Summarizer with Streamlit

## Project Overview
This project is a web application for summarizing text and documents using the Streamlit framework. It leverages Natural Language Processing (NLP) techniques to extract the most important sentences from a given text, providing a concise summary. Users can input text directly or upload documents for summarization. The summarized text can be downloaded in various formats such as plain text, PDF, or DOCX.

## Key Features
1. **Text Summarization:**
   - Users can input text directly into the application.
   - The application processes the text and generates a summary.
   - The summary, along with input and summary word counts, is displayed.

2. **Document Summarization:**
   - Users can upload documents in TXT, PDF, or DOCX formats.
   - The application extracts text from the uploaded document and generates a summary.
   - The summary, along with input and summary word counts, is displayed.

3. **Download Options:**
   - Summaries can be downloaded in multiple formats:
     - Plain text (TXT)
     - PDF
     - DOCX

## Technical Details
- **Libraries Used:**
  - **Streamlit:** For building the web application interface.
  - **NLTK:** For text processing and summarization.
  - **FPDF:** For generating PDF files.
  - **python-docx:** For generating DOCX files.
  - **PyPDF2:** For reading PDF files.
  
- **Summarization Process:**
  - Tokenize the text into words and sentences.
  - Remove stopwords and calculate word frequencies.
  - Score sentences based on the frequency of significant words.
  - Select top sentences to form the summary.

- **File Handling:**
  - For plain text files, read and decode the content.
  - For PDF files, extract text from each page.
  - For DOCX files, extract text from each paragraph.

## User Interface
- **Text Summarizer:**
  - Text area for users to input text.
  - Option to select the download format (Text, PDF, DOCX).
  - Button to initiate the summarization process.
  - Display area for the summary and related statistics.
  - Download buttons for the selected format.

- **Document Summarizer:**
  - File uploader for users to upload documents.
  - Option to select the download format (Text, PDF, DOCX).
  - Button to initiate the summarization process.
  - Display area for the summary and related statistics.
  - Download buttons for the selected format.

## How to Run the Application
1. Install the required libraries:
   ```sh
   pip install streamlit nltk fpdf python-docx PyPDF2


