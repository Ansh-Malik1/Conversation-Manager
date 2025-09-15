# Chat Extraction and Schema Validation Pipeline

This project implements a conversational pipeline where a chatbot extracts structured user information from natural language chats. The extracted information is validated against a predefined JSON schema to ensure correctness and reliability.  

---

## Features

- **Chat Simulation**: Input sample chat conversations with the assistant.  
- **Information Extraction**: Extracts fields like `name`, `age`, `email`, `phone`, and `location`.  
- **Schema Validation**: Uses `jsonschema.Draft7Validator` to validate the extracted data against a strict schema.  
- **Error Handling**: Captures validation and API errors (e.g., invalid age, missing fields) and reports them clearly.  
- **Readable Error Reporting**: Provides structured, human-readable validation errors (e.g., `"age must be <= 120 but found 150"`).  
- **Truncation Support**: Conversation history can be truncated by words, tokens or tunrs to manage context size.
- **History Summarization**: Conversation history gets summarize automatically after every k-th run and replaces the older version. 

---


## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/your-username/chat-extraction-pipeline.git
cd chat-extraction-pipeline
```
Install the dependencies and run

## Dependencies
groq

jsonschema

pprint

jupyter

Install them via:
```
pip install groq jsonschema pprintpp jupyter
```

## Future Improvements
Automate chat ingestion instead of manual input.

Enhance schema with more complex validations.

Integrate with a database for storing validated records.

#### Note: Refer to collab notebook for in depth code explanation and working

