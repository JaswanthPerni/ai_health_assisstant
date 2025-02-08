# Healthcare Assistant Chatbot

This is a simple Healthcare Assistant Chatbot built using Streamlit and the `distilgpt2` text-generation model from Hugging Face's Transformers library. The chatbot can provide basic responses to healthcare-related queries and generate text responses for other inputs.

## Features
- Recognizes keywords like "symptom", "appointment", and "medication" to provide predefined responses.
- Uses the `distilgpt2` model for generating responses to general queries.
- Interactive Streamlit interface for user-friendly interaction.

## Installation

To run this chatbot locally, follow these steps:

1. Clone this repository:
   ```bash
   git clone https://github.com/JaswanthPerni/ai_health_assisstant.git
   cd ai_health_assisstant
   ```
2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Requirements

Make sure you have the following Python libraries installed:
```txt
streamlit
nltk
transformers
```
If not, install them using:
```bash
pip install streamlit nltk transformers
```

Additionally, ensure that the NLTK stopwords and tokenizer data are downloaded:
```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```

## Usage

Run the chatbot using the following command:
```bash
streamlit run chatbot.py
```
This will start a local Streamlit web app where you can interact with the chatbot.

## Project Structure
```
ai_health_assisstant/
│── chatbot.py         # Main chatbot script
│── requirements.txt   # List of dependencies
│── README.md          # Project documentation
```

## Future Enhancements
- Improve the model's accuracy by fine-tuning it with healthcare-specific data.
- Integrate an API for real-time medical information retrieval.
- Add voice input and response capabilities.

## Contributing
Feel free to fork this repository and contribute improvements via pull requests.

Developed with ❤️ using Streamlit and Transformers.

