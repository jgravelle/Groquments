# Groquments
![image](https://github.com/user-attachments/assets/a7e50e52-b8e9-4198-a2b2-586f693e2316)

Groquments is a simple demonstration project showcasing how easily PocketGroq can help developers integrate Groq's powerful AI capabilities into their Python projects. This project provides a basic implementation of an AI-powered document field mapping tool.

**IMPORTANT**: Groquments is a demonstration project and is not intended for production use. It serves as an example of PocketGroq integration and should be used for learning and experimentation purposes only.

## Features

- Read source and target .docx documents
- Use AI to intelligently map fields between documents
- Generate JavaScript representation of the source document
- Fill out target document based on AI-generated field mapping
- Save the filled document as a new .docx file

## Prerequisites

- Python 3.7 or higher
- A Groq API key (sign up at [https://console.groq.com](https://console.groq.com) to obtain one)

## Setup

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/groquments.git
   cd groquments
   ```

2. Create and activate a virtual environment:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

4. Set up your environment variables:
   - Rename `.env.sample` to `.env`
   - Open `.env` and replace `your_groq_api_key_here` with your actual Groq API key

## Usage

1. Prepare your source and target .docx documents:
   - Place them in the `input_documents` directory (create it if it doesn't exist)
   - Ensure both documents have a clear structure with labeled fields

2. Run the Groquments script:
   ```
   python groquments.py
   ```

3. Follow the prompts to select your source and target documents

4. The script will process the documents and save the filled target document in the `output_documents` directory

## How It Works

1. Groquments reads the source and target documents
2. It generates a JavaScript representation of the source document
3. The script uses the Groq AI model (via PocketGroq) to intelligently map fields between the documents
4. Based on this mapping, it fills out the target document
5. Finally, it saves the filled document as a new .docx file

## Limitations

- This is a demonstration project and may not handle all document structures or field types
- The AI-based field mapping is experimental and may not always produce perfect results
- Error handling is basic and may not cover all edge cases

## Contributing

As this is a demonstration project, we're not actively seeking contributions. However, feel free to fork the repository and experiment with your own enhancements!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This project uses [PocketGroq](https://github.com/jgravelle/pocketgroq) to integrate Groq's AI capabilities
- Document handling is powered by the [python-docx](https://python-docx.readthedocs.io/) library

Remember, Groquments is a simple demo to illustrate PocketGroq integration. For production use, always implement proper error handling, security measures, and thorough testing.py2md
