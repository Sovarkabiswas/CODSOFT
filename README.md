# CODSOFT
New Repository 
# Function to get a response based on user input
def get_response(user_input):
    # Convert user input to lowercase for case-insensitive matching
    user_input = user_input.lower()
    
    # Check for specific user queries
    if "hello" in user_input:
        return "Hello! How can I assist you today?"
    elif "how are you" in user_input:
        return "I'm just a computer program, so I don't have feelings, but thanks for asking!"
    elif "goodbye" in user_input:
        return "Goodbye! Have a great day."
    else:
        return "I'm not sure how to respond to that."

# Main loop for chatbot interaction
print("Simple Chatbot: Type 'goodbye' to exit.")
while True:
    user_input = input("You: ")
    if user_input.lower() == "goodbye":
        print("Simple Chatbot: Goodbye!")
        break
    response = get_response(user_input)
    print("Simple Chatbot:", response)
