# Translation Model Web Interface

This project provides a web interface to interact with a custom-trained translation model using FastAPI. The model translates text between English and several Indian languages.

## Project Structure

```
D:\CubeAI\Translator_Model\translation_model_project\
├── main.py
├── templates\
│   └── index.html
└── static\
    ├── css\
    │   └── styles.css
    └── js\
        └── main.js
```

## Features

- Translate text between English and multiple Indian languages.
- Interactive web interface for easy testing and use.
- Supports languages: Hindi, Bengali, Telugu, Marathi, Tamil, Gujarati, Malayalam, Kannada, Odia, Punjabi.

## Prerequisites

Ensure you have the following installed:
- Python 3.7 or higher
- Uvicorn
- FastAPI
- Transformers
- SentencePiece

You can install these dependencies using pip:

```bash
pip install uvicorn fastapi transformers sentencepiece
```

## Setup

1. **Clone the Repository**

   ```bash
   git clone <repository_url>
   cd translation_model_project
   ```

2. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Download and Save the Model**

   Place your pre-trained translation model files in `D:\CubeAI\Translator_Model\translation_model_project\translator_model`.

4. **Run the FastAPI Server**

   ```bash
   uvicorn main:app --reload
   ```

5. **Open the Web Interface**

   Navigate to `http://127.0.0.1:8000` in your web browser to access the translation interface.

## Usage

- **Text to Translate**: Enter the text you want to translate in the provided text area.
- **Select Target Language**: Choose the language you want to translate to from the dropdown menu.
- **Translate**: Click the "Translate" button to get the translated text.

## Code Overview

- **`main.py`**: The main FastAPI application that handles routing and translation logic.
- **`templates/index.html`**: The HTML template for the user interface.
- **`static/css/styles.css`**: The CSS file for styling the web interface.
- **`static/js/main.js`**: The JavaScript file for handling form submissions and updating the page with the translated text.

## Troubleshooting

- **500 Internal Server Error**: Ensure all file paths are correct and the model is properly loaded. Check the FastAPI server logs for detailed error messages.
- **Question Marks in Translation**: Verify the encoding of your text files and ensure UTF-8 is used throughout the project.

## Contributing

Feel free to open issues or submit pull requests if you encounter any bugs or have suggestions for improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

### Additional Notes

1. **Replace `<repository_url>`** with the actual URL of your GitHub repository.
2. **Create a `requirements.txt`** file if you haven't already, listing all the Python dependencies for easy installation:
   
   ```
   uvicorn
   fastapi
   transformers
   sentencepiece
   ```

This README provides a comprehensive guide for users and contributors, making it easier to understand and work with your project.
