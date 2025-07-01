# AnsibleSWEAssessment

Leo's Ansible SWE Assessment Submission

## Overview

This repository contains Leo's submission for the Ansible Software Engineering Assessment. The project demonstrates proficiency in Python programming, Google API integration, and document processing automation. Used Claude AI heavily.

## Project Contents

- **`Ansible.ipynb`** - Jupyter notebook containing the main implementation
- **`Assessment/`** - Assessment directory (currently empty)

## Features

The main implementation in `Ansible.ipynb` includes:

### Google Docs API Integration
- Authentication with Google Docs API using Google Colab
- Document creation and management
- Batch updating with API rate limiting

### Markdown to Google Docs Converter
- Converts Markdown text to formatted Google Docs
- Supports multiple formatting features:
  - Headers (H1, H2, H3)
  - Bullet points with nested indentation
  - Checkboxes (completed and uncompleted)
  - @mentions with special formatting
  - Footer styling for metadata

### Error Handling
- Comprehensive exception handling for API calls
- Rate limiting management
- Authentication error recovery

## Key Functions

- `authenticate_google_docs()` - Handles Google API authentication
- `create_google_doc(service, title)` - Creates new Google Docs
- `update_google_doc(service, doc_id, requests)` - Applies formatting updates
- `parse_markdown(md_text)` - Converts Markdown to Google Docs API requests

## Example Usage

The notebook includes a complete example that converts meeting notes from Markdown format to a fully formatted Google Doc with proper styling, bullet points, and @mentions.

## Dependencies

- `google.auth` - Google authentication
- `googleapiclient` - Google API client library
- `google.colab` - Colab authentication
- `markdown` - Markdown processing
- `json`, `re`, `unittest` - Standard Python libraries

## Running the Code

1. Open `Ansible.ipynb` in Google Colab
2. Run all cells to execute the complete workflow
3. Authenticate when prompted
4. The script will create a formatted Google Doc from the example Markdown content
