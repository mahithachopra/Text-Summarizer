# AI-Powered Text Summarizer

## Overview
The **AI-Powered Text Summarizer** is a Streamlit-based application that allows users to summarize lengthy articles, PDFs, DOCX, and text files using AI-powered Natural Language Processing (NLP). The tool utilizes the **Sumy** library for text summarization and supports **PyPDF2** and **python-docx** for text extraction.

## Features
- Summarizes text from user input, PDF files, DOCX files, and plain text files.
- Uses **TextRankSummarizer** from Sumy for high-quality AI-powered summaries.
- Allows users to select the number of sentences for the summary.
- Provides an interactive **Streamlit** UI with customizable styling.
- Enables downloading the summary in **TXT, DOCX, and PDF** formats.

## Technologies Used
- **Python**: Core programming language.
- **Streamlit**: Web application framework.
- **Sumy**: Text summarization library.
- **PyPDF2**: PDF text extraction.
- **nltk**: Tokenization for text processing.
- **python-docx**: DOCX file text extraction.
- **PIL**: Image handling for UI.

## Installation

### Prerequisites
Ensure you have Python 3.7+ installed. Then, install the required dependencies:

pip install -r requirements.txt

Download the necessary NLTK tokenizer:
import nltk
nltk.download('punkt_tab')

## Usage
1. **Run the application**:
streamlit run app.py

2. **Choose Input Method**:
   - Enter text manually.
   - Upload a **TXT, PDF, or DOCX** file.

3. **Adjust Summary Settings**:
   - Select the number of sentences for summarization (5-25).

4. **Generate Summary**:
   - Click **'Generate Summary'** to process the text.

5. **Download Summary**:
   - Save the summary as **TXT, DOCX, or PDF**.

## Code Structure

**summarize_text(text, num_sentences=10)**: Summarizes the given text using TextRank.
**extract_text_from_pdf(uploaded_file)**: Extracts text from uploaded PDF files.
**extract_text_from_docx(uploaded_file)**: Extracts text from uploaded DOCX files.
**main()**: Streamlit application UI and controls.

## Known Issues
- Some PDFs may have text extraction limitations.
- Complex formatting in DOCX files may not be preserved.

## Contribution
Feel free to fork and enhance the project. Pull requests are welcome!

