# 🦙💬 Llama 3 Chatbot

Welcome to the Llama 3 Chatbot application! This Streamlit app utilizes the Llama 3.1 model from the `ctransformers` library to provide a conversational AI experience. Below you'll find information on how to set up and use this app.

## Features

- **Interactive Chatbot**: Engage in a conversation with the Llama 3 model.
- **Adjustable Parameters**: Configure the chatbot's temperature and top_p settings using sliders.
- **Chat History Management**: Clear the chat history at any time.
- **Dynamic Responses**: Receive responses based on user input with contextual understanding.

## Requirements

To run this application, you'll need:

- Python 3.7 or later
- Streamlit
- ctransformers

You can install the required packages using pip:

```bash
pip install streamlit ctransformers
```

## How to Run

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Streamlit App**:
   ```bash
   streamlit run app.py
   ```

   Replace `app.py` with the name of your script if it's different.

## Usage

1. **Set Parameters**: Use the sliders in the sidebar to adjust the `temperature` and `top_p` parameters to control the creativity and diversity of the chatbot's responses.

2. **Interact with the Chatbot**:
   - Type your message in the input box and press Enter.
   - The chatbot will respond to your input based on the adjusted parameters.

3. **Clear Chat History**: Use the 'Clear Chat History' button in the sidebar to start a new conversation.

## Code Overview

- **Model Loading**: The `ChatModel` function initializes the Llama 3.1 model with parameters set through the sidebar sliders.
  
- **Chat History**: Stored in `st.session_state.messages`, allowing the chat history to persist across interactions.

- **Message Handling**: Messages are displayed in the chat window and managed to generate appropriate responses.

- **Response Generation**: The `generate_llama2_response` function handles crafting the prompt and generating the response based on the model's output.

## Customization

You can modify the following aspects of the app:

- **Model Parameters**: Adjust the `temperature` and `top_p` sliders to fine-tune the chatbot's responses.
- **Model Choice**: Change the model by modifying the `from_pretrained` method's arguments in the `ChatModel` function.

## Troubleshooting

- **Model Loading Issues**: Ensure that you have the correct model path and that all dependencies are properly installed.
- **Performance**: For slower response times, consider adjusting the `temperature` and `top_p` parameters or checking your system's resources.

## Contributing

Feel free to open issues or submit pull requests if you have suggestions or improvements for the app.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, please reach out to [sriniagt.cse@gmail.com](mailto:sriniagt.cse@gmail.com).

Enjoy chatting with Llama 3! 🦙💬

---
