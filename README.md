# PDF Processor Application

This application allows users to upload PDF documents, extract text using OCR, and generate summaries using the Grok X AI API.

## Features

- PDF document upload
- Text extraction using OCR (Magic_pdf / MinerU)
- Text summarization using Grok X AI API
- Simple web interface for uploading and viewing results
- Asynchronous processing with a message queue system
- Local file storage for documents, extracted text, and summaries

## Project Structure

```plaintext
pdf-processor/
│
├── app.py                    # Main Flask application
├── requirements.txt          # Python dependencies
├── config.py                 # Configuration settings
│
├── static/                   # Static files for web interface
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── main.js
│
├── templates/                # HTML templates
│   ├── index.html
│   └── results.html
│
├── services/                 # Service modules
│   ├── __init__.py
│   ├── ocr_service.py        # OCR with MinerU integration
│   ├── summary_service.py    # LLM summary with Grok X API
│   ├── storage_service.py    # File storage handling
│   └── message_service.py    # Simple message queue implementation
│
└── uploads/                  # Local storage for uploaded files
    ├── pdfs/
    ├── text/
    └── summaries/
```
