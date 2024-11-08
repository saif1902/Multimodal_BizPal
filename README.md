# BizPal Multimodal RAG
This project leverages the power of Multimodal Retrieval Augmented Generation (RAG) to provide comprehensive and context-aware answers related to the BizPal program.

## Overview
The project encompasses the following key steps:

1. **Data Collection**: Gathers information from various sources including YouTube videos, PDF documents, and images.
2. **Data Processing**: Extracts relevant data such as text, audio transcriptions, image metadata, and tables.
3. **Embedding and Storage**: Embeds processed data using OpenAI's text-embedding-ada-002 model and stores it in a Weaviate database.
4. **Querying and Retrieval**: Searches the database using semantic similarity to find relevant information.
5. **Response Generation**: Integrates retrieved information to provide insightful answers to user questions using the GPT-4 model.

## Key Features
* Multimodal search across different data types.
* Rich context-aware responses.
* Utilizes advanced technologies like Weaviate and GPT-4.
* Streamlined workflow for data processing and analysis.


## Dependencies
* ffmpeg-python
* yt_dlp
* openai-whisper
* pdfminer.six
* pillow-heif
* matplotlib
* tesseract-ocr
* unstructured-inference
* unstructured-pytesseract
* pi-heif
* unstructured
* langchain-core
* langchain-openai
* weaviate-client
* openai
* textwrap3

To install dependencies, run: bash pip install -r requirements.txt

**Note**: The project requires API keys for OpenAI, Weaviate Cloud Services (WCS) and  Google Drive. Please set them as environment variables.

## Usage
1. Install the required dependencies.
2. Set up environment variables.
3. Update file paths for data sources.
4. Run the notebook cells sequentially.

## Example
To query the model, use the following code: 
python query = "What are the main features of BizPal?" response = bizpal_analysis(query) print(response)


**Disclaimer:** This project is a proof-of-concept, and has certain limitations and possible inaccuracies.
