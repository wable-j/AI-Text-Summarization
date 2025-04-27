# AI Text Summarization

A powerful AI-based text summarization application that helps condense long documents, articles, and other content into concise, readable summaries.

## Overview

This project provides an interactive web application for generating summaries from various input sources using state-of-the-art natural language processing techniques. It features a React-based frontend and a Python FastAPI backend that leverages Hugging Face Transformers models for summarization.

![AI Text Summarization Interface](https://placeholder-for-screenshot.png)

## Features

- **Multiple Input Types**:
  - Direct text input
  - Voice/speech recording
  - URL content summarization
  - PDF document summarization

- **Flexible Summarization Methods**:
  - Abstractive: AI-generated summary that paraphrases the original content
  - Extractive: Selects and combines the most important sentences from the original text

- **Customizable Styles**:
  - Various summarization styles for different needs (concise, detailed, creative, academic, etc.)
  - Adjustable length controls

- **Interactive UI**:
  - Step-by-step workflow
  - Talking avatar to read summaries aloud
  - Particle background for visual appeal
  - Responsive design

## Tech Stack

### Frontend
- React 19
- Three.js for 3D rendering
- TensorFlow.js for face tracking
- React Three Fiber/Drei

### Backend
- FastAPI
- PyTorch
- Hugging Face Transformers
- NLTK and other NLP libraries

## Installation & Setup

### Prerequisites
- Node.js (v16+)
- Python (v3.9+)
- pip and npm package managers

### Backend Setup

1. Navigate to the backend directory:
   ```
   cd backend
   ```

2. Create a virtual environment (recommended):
   ```
   python -m venv venv
   ```

3. Activate the virtual environment:
   - Windows:
     ```
     venv\Scripts\activate
     ```
   - macOS/Linux:
     ```
     source venv/bin/activate
     ```

4. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

5. Start the backend server:
   ```
   uvicorn main:app --reload
   ```
   The API will be available at http://localhost:8000

### Frontend Setup

1. Navigate to the frontend directory:
   ```
   cd frontend
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Start the development server:
   ```
   npm start
   ```
   The application will open at http://localhost:3000

## Usage

1. **Start the Application**:
   - Click "Start Summarizing" on the introduction page

2. **Select Input Type**:
   - Text: Paste text directly
   - Speech: Record and transcribe your voice
   - URL: Enter a webpage URL to summarize
   - PDF: Upload a PDF document

3. **Choose Summarization Method**:
   - Abstractive: AI-generated paraphrasing
   - Extractive: Key sentence selection

4. **Select Summarization Style**:
   - Different options available based on the selected method

5. **Enter Content**:
   - Provide the content to summarize based on selected input type
   - Adjust minimum and maximum length settings if needed

6. **Generate Summary**:
   - Click "Generate Summary" and wait for processing
   - View the results with statistics and a talking avatar reading the summary

## API Documentation

The backend provides several endpoints:

- `GET /`: API information
- `GET /styles`: Get available summarization styles
- `POST /summarize/text`: Summarize plain text
- `POST /summarize/url`: Summarize content from URL
- `POST /summarize/pdf`: Summarize content from PDF
- `POST /translate`: Translate text to another language

Swagger UI documentation is available at http://localhost:8000/docs when the backend is running.

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## License

[MIT License](LICENSE)

## Acknowledgments

- This project uses Hugging Face Transformers for NLP tasks
- Frontend animations powered by Three.js
- Voice features use the Web Speech API