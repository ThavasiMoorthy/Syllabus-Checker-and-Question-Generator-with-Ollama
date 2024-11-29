# Automated Question Paper Processing System

This project provides a streamlined pipeline for processing question papers and syllabi using **Python** and the **Ollama** API. It extracts, corrects, aligns, and generates relevant content for academic purposes, ensuring grammatical accuracy and syllabus alignment.

## Features

- Extracts text from `.txt` and `.pdf` files.
- Corrects grammatical errors and spelling mistakes in question papers.
- Identifies irrelevant questions based on the provided syllabus.
- Generates replacement questions aligned with the syllabus using Bloom's Taxonomy.
- Produces revised question papers with corrected and relevant questions.
- Summarizes the syllabus in concise terms for better understanding.
- Outputs responses in a user-friendly, streamed format.

## Tech Stack

- **Python**: Core programming language.
- **PyPDF2**: For text extraction from PDF files.
- **Ollama API**: For natural language processing tasks.
- **Time**: For controlled, word-by-word console printing.

## How It Works

1. **Text Extraction**: Reads text from a syllabus file (`ML1301.txt`) and a question paper file (`model23.txt`).
2. **Question Processing**:
   - Corrects grammar and spelling errors in the extracted questions.
   - Identifies questions irrelevant to the syllabus.
   - Generates syllabus-aligned replacement questions using Bloom's Taxonomy.
3. **Revision**: Updates the question paper by replacing irrelevant questions with the newly generated ones.
4. **Syllabus Summarization**: Summarizes the syllabus into 5-10 sentences for quick understanding.

## Code Structure

- **`extract_text_from_txt(file_path)`**: Extracts plain text from `.txt` files.
- **`printer(v)`**: Displays text in a word-by-word streaming style in the console.
- **`processone(q)`**: Corrects and formats the extracted questions.
- **`check(question, syllabus)`**: Identifies irrelevant questions.
- **`generate_replacement_questions(irrelevant, syllabus)`**: Creates syllabus-aligned questions.
- **`revised(question, irrelevant, replacement)`**: Generates the updated question paper.
- **`understand(s)`**: Summarizes the syllabus content.
