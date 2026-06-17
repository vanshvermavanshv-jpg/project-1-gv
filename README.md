# project-1-gv





print("=" * 50)
print("        Welcome to AI Chatbot")
print("=" * 50)
print("Type 'exit' anytime to end the conversation.\n")

user_name = input("Enter your name: ")
print(f"\nHello {user_name}! I am your AI Chatbot.")
print("How can I help you today?\n")

while True:

    user_input = input("You: ").lower().strip()

    # Exit Commands
    if user_input in ["exit", "quit", "bye", "goodbye"]:
        print("Bot: Thank you for chatting with me. Have a great day!")
        break

    # Greetings
    elif user_input in ["hi", "hello", "hey", "hii"]:
        print(f"Bot: Hello {user_name}! Nice to meet you.")

    # Asking Name
    elif "your name" in user_input:
        print("Bot: My name is DecodeBot, a simple rule-based AI chatbot.")

    # Asking Age
    elif "age" in user_input:
        print("Bot: I don't have an age because I am a computer program.")

    # Asking About AI
    elif "artificial intelligence" in user_input or "ai" in user_input:
        print("Bot: Artificial Intelligence enables machines to perform tasks that usually require human intelligence.")

    # Asking Time
    elif "time" in user_input:
        from datetime import datetime
        current_time = datetime.now().strftime("%H:%M:%S")
        print("Bot: Current time is", current_time)

    # Asking Date
    elif "date" in user_input:
        from datetime import date
        today = date.today()
        print("Bot: Today's date is", today)

    # Asking About Decode Labs
    elif "decode labs" in user_input:
        print("Bot: Decode Labs provides internship programs and project-based learning opportunities.")

    # Help Section
    elif "help" in user_input:
        print("Bot: You can ask me about:")
        print("- My name")
        print("- AI")
        print("- Time")
        print("- Date")
        print("- Decode Labs")
        print("- Greetings")

    # Thank You
    elif "thank" in user_input:
        print("Bot: You're welcome! Happy to help.")

    # Default Response
    else:
        print("Bot: Sorry, I don't understand that yet. Please try another question.")
