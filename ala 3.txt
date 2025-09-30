# doctor_chatbot.py
# Simple rule-based chatbot for doctor-patient communication

print("DoctorBot: Hello! I am DoctorBot. How can I help you today?")
print("Type 'bye' to end the chat.\n")

while True:
    user_input = input("You: ").lower()

    if "hello" in user_input or "hi" in user_input:
        print("DoctorBot: Hello! How are you feeling today?")

    elif "fever" in user_input:
        print("DoctorBot: I see. Do you also have symptoms like cough or headache?")

    elif "cough" in user_input:
        print("DoctorBot: You might have a common cold. Drink warm fluids and take rest.")

    elif "headache" in user_input:
        print("DoctorBot: Make sure you are hydrated. If pain continues, consider mild medication.")

    elif "stomach pain" in user_input or "stomachache" in user_input:
        print("DoctorBot: Try to rest and avoid heavy food. If pain is severe, you should visit a doctor.")

    elif "covid" in user_input:
        print("DoctorBot: If you have fever, cough, and breathing issues, please get a COVID-19 test immediately.")

    elif "thank you" in user_input or "thanks" in user_input:
        print("DoctorBot: You're welcome! Take care of your health.")

    elif "bye" in user_input:
        print("DoctorBot: Goodbye! Wishing you good health.")
        break
    else:
        print("DoctorBot: I'm not sure about that. Please provide more details about your symptoms.")
