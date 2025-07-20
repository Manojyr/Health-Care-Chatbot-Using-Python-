# Health-Care-Chatbot-Using-Python-
🧠 Health-Care Chatbot using Python, NLTK & TensorFlow
A smart AI-powered chatbot that interacts with users, detects symptoms, and provides basic healthcare advice, medication suggestions, prevention tips, and links to doctor consultation services. Ideal for early-stage symptom assessment and awareness.

🚀 Project Features
🤖 Conversational chatbot that understands user inputs (e.g. "I have a headache", "How to prevent diabetes?")

💬 Pre-trained intent classification using TensorFlow

🧠 Natural Language Processing using NLTK for tokenization and lemmatization

💊 Health conditions included: Fever, Cold, Diabetes, Asthma, Depression, Headache

📌 Provides:

Symptom-based disease detection

Medication recommendations

Diet & prevention tips

Links for online doctor consultations

📁 Simple console-based interface (Tkinter GUI can be added)

📁 Project Structure
bash
Copy code
Health-Care-Chatbot/
│
├── intents.json            # All user intents and chatbot responses
├── chatbot_py.py           # Main chatbot script
├── train_chatbot.py        # Trains the model using intents.json
├── chatbotmodel.h5         # Saved Keras model after training
├── words.pkl               # Vocabulary tokens (used for inference)
├── classes.pkl             # Intent tags list
├── README.md               # Project documentation
└── venv/                   # Virtual environment (optional)
📦 Requirements
Python 3.10 or higher

TensorFlow

NLTK

NumPy

Pickle (Python standard library)

To install required libraries:

bash
Copy code
pip install nltk tensorflow numpy
You’ll also need to download NLTK data:

python
Copy code
import nltk
nltk.download('punkt')
nltk.download('wordnet')
⚙️ How to Run
🔹 Step 1: Train the Model
bash
Copy code
python train_chatbot.py
This will create:

chatbotmodel.h5

words.pkl

classes.pkl

🔹 Step 2: Run the Chatbot
bash
Copy code
python chatbot_py.py
Then start chatting:

vbnet
Copy code
You: I have a fever
MedBot: It seems that you are suffering from fever
📚 Sample Interactions
User Input	Chatbot Response
I have a headache	Try resting in a quiet, dark room. Stay hydrated and consider taking a pain reliever.
I feel tired and sad	It seems that you are suffering from depression
What should I eat if I have diabetes?	Suggested foods: Leafy greens, Avocados, Eggs
Can I consult a doctor?	You can consult online: 1mg, TataHealth, DocOnline

🔮 Future Enhancements
Add GUI with Tkinter or PyQt

Enable speech-to-text and text-to-speech

Deploy to web using Flask or Streamlit

Use a more advanced NLP model (like BERT)

Integrate WhatsApp/Telegram API for real use

🙋‍♂️ Author
Manoj Y R
Built as part of a smart healthcare initiative project.
