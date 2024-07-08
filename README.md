# ChatBot
This repository contains the code for a chatbot built using TensorFlow/Keras, NLTK, and Tkinter. The chatbot is designed to understand and respond to user inputs based on predefined intents.
# Table of Contents
- Installation
- Usage
- Training the Model
- Running the Chatbot
- Dependencies
# Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/ParthChande/ChatBot
   ```
   ```sh
   cd chatbot-project
   ```
3. Install the required packages:
   ```sh
   pip install -r requirements.txt
   ```
# Usage
1. Ensure you have the intents.json file in the project directory. This file contains the predefined intents and responses.
2. Train the model and run the chatbotusing the provided script.
   
   ``ChatBot.ipynb``
# Training the Model and running the ChatBot
1. Load and preprocess the data from intents.json.
2. Train a neural network using TensorFlow/Keras to classify user inputs into predefined intents.
3. Save the trained model and preprocessing data
4. After training the model, you can run the chatbot application using Tkinter. The chatbot will use the trained model to predict user intents and respond accordingly.
# Dependencies
- Python 3.6+
- NLTK
- TensorFlow/Keras
- NumPy
- Tkinter
# Code Overview
__Preprocessing__

The script preprocesses the data from intents.json:

- Tokenizes and lemmatizes the patterns.
- Creates a bag of words model.
- Converts class labels to one-hot encoding.
__Model Training__

The script trains a Sequential model with the following architecture:

- Input layer with 128 neurons and ReLU activation.
- Dropout layer with 50% dropout rate.
- Hidden layer with 64 neurons and ReLU activation.
- Dropout layer with 50% dropout rate.
- Output layer with softmax activation.
  
The model is trained using stochastic gradient descent (SGD) with a learning rate of 0.01, decay of 1e-6, momentum of 0.9, and Nesterov accelerated gradient.

![image](https://github.com/ParthChande/ChatBot/assets/119730313/90bf4177-89cc-4a76-aa93-df506336bc9b)
![image](https://github.com/ParthChande/ChatBot/assets/119730313/2cd19220-a1a9-41ae-b871-c7d949805583)



__Chatbot Application__

The script creates a simple GUI using Tkinter:

- Takes user input from a text box.
- Predicts the intent using the trained model.
- Displays the response in the chat log.

![image](https://github.com/ParthChande/ChatBot/assets/119730313/760f63d9-db39-476e-a156-2749b76ba238)
