# AI-CHATBOT-WITH-NLP

COMPANY NAME - CODETECH IT SOLUTIONS

STUDENT NAME - VIKRAM SHIVABASAPPA TIGADI

INTERN ID - CT06DY1737

MENTOR NAME - NEELA SANTOSH

DURATION - 6 WEEKS

BATCH - AG26

# ============================
# AI Chatbot using NLTK (NLP)
# ============================

# Step 1: Import necessary libraries
import nltk
from nltk.chat.util import Chat, reflections

# Step 2: Download NLTK data (only needed once)
nltk.download('punkt')

# Step 3: Define patterns and responses using regular expressions
pairs = [
    [
        r"hi|hello|hey",
        ["Hello!", "Hi there!", "Hey! How can I help you today?"]
    ],
    [
        r"what is your name ?",
        ["I'm an AI chatbot created with NLTK."]
    ],
    [
        r"how are you ?",
        ["I'm doing well, thank you!", "I'm great! How about you?"]
    ],
    [
        r"what can you do ?",
        ["I can answer simple questions and show how a chatbot works using NLP."]
    ],
    [
        r"who (created|developed) you ?",
        ["I was created by a developer using Python and NLTK."]
    ],
    [
        r"(.*)(weather|temperature)(.*)",
        ["Sorry, I can't fetch real-time weather. Try asking Google :)"]
    ],
    [
        r"(.*)(your name)(.*)",
        ["My name is Chatbot. Nice to meet you!"]
    ],
    [
        r"(.*) (help|support) (.*)",
        ["Sure, I'm here to help! What do you need assistance with?"]
    ],
    [
        r"(.*)",
        ["I'm not sure I understand. Can you rephrase that?"]
    ]
]

# Step 4: Define the chatbot function
def chatbot():
    print("🤖 Hello! I'm your AI Chatbot.")
    print("💬 Type 'quit' to exit anytime.\n")
    
    chat = Chat(pairs, reflections)
    chat.converse()

# Step 5: Run the chatbot
if __name__ == "__main__":
    chatbot()

output:🤖 Hello! I'm your AI Chatbot.
💬 Type 'quit' to exit anytime.

> hello
Hi there!

> what is your name ?
I'm an AI chatbot created with NLTK.

> how are you ?
I'm doing well, thank you!

> what can you do ?
I can answer simple questions and show how a chatbot works using NLP.

> who developed you ?
I was created by a developer using Python and NLTK.

> tell me about the weather
Sorry, I can't fetch real-time weather. Try asking Google :)

> i need some help
Sure, I'm here to help! What do you need assistance with?

> can you learn?
I'm not sure I understand. Can you rephrase that?

> quit
>
> Objectives

1]Understand and implement basic NLP techniques using Python.

2]Create a simple AI chatbot capable of interacting with users through text.

3]Use pattern matching and regular expressions to detect user intent.

4]Utilize NLTK’s built-in tools for tokenization and conversational logic.

5]Demonstrate how NLP libraries (like NLTK) can be used for rule-based chatbots

