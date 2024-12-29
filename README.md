# F1_CHATBOT_Streamlit

A simple, interactive chatbot built with Python and Streamlit that answers questions about Formula 1 racing. The chatbot uses natural language processing and TF-IDF vectorization to find relevant responses from a knowledge base about F1.

## Features

- Web-based interface using Streamlit
- Natural language processing with NLTK
- TF-IDF vectorization for text similarity
- Persistent chat history
- Custom F1 racing knowledge base
- Real-time response generation

## Prerequisites

Before running this project, make sure you have Python 3.7+ installed on your system. You can check your Python version by running:
```bash
python --version
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/AchourTen/F1_CHATBOT_Streamlit.git
cd F1_CHATBOT_Streamlit
```

2. Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate
```

3. Install the required packages:
```bash
pip install -r requirements.txt
```

## Project Structure

```
f1-chatbot/
│
├── chatbot.py          # Main application file
├── F1.txt             # Knowledge base about Formula 1
├── requirements.txt    # Project dependencies
└── README.md          # Project documentation
```

## Running the Application

1. Make sure you're in the project directory and your virtual environment is activated (if using one)

2. Run the Streamlit app:
```bash
streamlit run chatbot.py
```

3. Open your web browser and go to the URL shown in the terminal (typically http://localhost:8501)

## Usage

1. Type your question about Formula 1 in the text input field
2. Press Enter or click the submit button
3. The chatbot will respond with relevant information from its knowledge base
4. Your chat history will be displayed and maintained throughout the session

Example questions you can ask:
- "What is DRS and how does it work?"
- "How many points do you get for winning a race?"
- "Who has won the most championships?"
- "What are the different tire compounds used in F1?"

## Dependencies

The project requires the following main packages:
- streamlit
- nltk
- scikit-learn
- numpy
- pandas

All dependencies are listed in `requirements.txt`.

## Creating requirements.txt

Run the following command to create your requirements.txt:
```bash
pip freeze > requirements.txt
```

## Customization

You can customize the chatbot by:
1. Modifying the F1.txt file to include different or additional information
2. Adjusting the similarity threshold in the `get_response` method
3. Adding more preprocessing steps in the `preprocess` method
4. Enhancing the user interface through Streamlit customization

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Future Upgrade 
Scraping information from Wiki and other site for more automation 

## Acknowledgments

- Data source: Compiled from various Formula 1 resources
- Built with [Streamlit](https://streamlit.io/)
- NLP processing with [NLTK](https://www.nltk.org/)
