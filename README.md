!pip install --upgrade openai==0.27.0
import openai

# Replace with your OpenAI API key
openai.api_key = "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"

def chat_with_gpt():
    print("Hi, welcome to Home LLC! How may I help you?")
!pip install --upgrade openai==0.27.0
import openai

# Replace with your OpenAI API key
openai.api_key = "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"

def chat_with_gpt():
    print("Hi, welcome to Home LLC! How may I help you?")

    # Predefined responses for specific questions
    predefined_responses = {
        "What should we know about your life story in a few sentences?": 
            "I have a journey filled with learning and growth, constantly evolving to provide the best solutions.",
        "What’s your #1 superpower?":
            "My #1 superpower is problem-solving. I'm adept at finding innovative solutions to complex challenges."
    }

    while True:
        user_input = input("You: ")
        if user_input.lower() == "exit":
            break

        if user_input in predefined_responses:
            print("Home LLC:", predefined_responses[user_input])
        else:
            # Use OpenAI API to generate a response
            response = openai.ChatCompletion.create(
                model="gpt-3.5-turbo",
                messages=[
                    {"role": "system", "content": "You are a helpful assistant."},
                    {"role": "user", "content": user_input}
                ]
            )
            print("Home LLC:", response.choices[0].message.content)


if __name__ == "__main__":
    chat_with_gpt()

# Replace with your OpenAI API key
openai.api_key = "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"

def chat_with_gpt():
    print("Hi, welcome to Home LLC! How may I help you?")

    # Predefined responses for specific questions
    predefined_responses = {
        "What should we know about your life story in a few sentences?": 
            "I have a journey filled with learning and growth, constantly evolving to provide the best solutions.",
        "What’s your #1 superpower?":
            "My #1 superpower is problem-solving. I'm adept at finding innovative solutions to complex challenges."
    }

    while True:
        user_input = input("You: ")
        if user_input.lower() == "exit":
            break

        if user_input in predefined_responses:
            print("Home LLC:", predefined_responses[user_input])
        else:
            # Use OpenAI API to generate a response
            response = openai.ChatCompletion.create(
                model="gpt-3.5-turbo",
                messages=[
                    {"role": "system", "content": "You are a helpful assistant."},
                    {"role": "user", "content": user_input}
                ]
            )
            print("Home LLC:", response.choices[0].message.content)

Home LLC AI Chatbot 
