# Emotion Detection System with Watson AI 🧠💬

An advanced Emotion Detection system that uses IBM's Watson AI Natural Language Understanding (NLU) API to analyze text and detect the emotional tone behind it. This project identifies key emotions such as joy, sadness, anger, fear, disgust, and surprise from user input.

## Features 🌟

- **Emotion Detection:** 🧠 Identifies the emotional tone behind text inputs, such as joy, sadness, anger, fear, disgust, and surprise.
- **Natural Language Processing (NLP):** 🤖 Utilizes IBM Watson's Natural Language Understanding API for accurate sentiment analysis and emotion classification.
- **Real-Time Feedback:** ⚡ Users can get immediate feedback about the emotions expressed in their input text.
- **Customizable:** 🔧 Easily adaptable for integration into various applications or chatbots to detect emotions from conversations.
- **Detailed Analysis:** 📊 Provides a detailed breakdown of emotions detected along with their intensity scores.

## Technologies Used 🛠️

- **IBM Watson NLU API:** 🧠 Provides deep sentiment and emotion analysis capabilities.
- **Python:** 🐍 Used for backend development and integration of the Watson API.
- **Flask:** 🖥️ A lightweight framework for creating a web application to handle API requests.
- **JavaScript/HTML/CSS:** 💻 For frontend user interaction (if building a web interface).
- **ngrok:** 🌍 If you want to make your Flask app accessible over the web for testing.

## How It Works 🚀

1. **Input Text:** 📝 The system receives text input from the user.
2. **Emotion Analysis:** 🧠 The text is sent to IBM Watson’s Natural Language Understanding API for emotion and sentiment analysis.
3. **Output Emotion:** 🌈 The detected emotion is then processed and returned to the user, with an optional confidence score showing the intensity of the detected emotion.
4. **Real-Time Feedback:** ⚡ The user receives a detailed report of detected emotions, including percentages and intensity for each emotion.

## Setup & Installation ⚙️

### Prerequisites

- **Python 3.x**
- **IBM Watson NLU API Key:** 🧠 You need an IBM Cloud account and an NLU instance for accessing the API key.
- **Flask:** A lightweight Python web framework.
- **ngrok (Optional):** For creating a publicly accessible URL to test the app locally.

### Steps to Install

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/emotion-detection-watson.git
   cd emotion-detection-watson
   ```

2. **Install Dependencies:**
   Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up IBM Watson NLU:**
   - Go to [IBM Watson NLU](https://cloud.ibm.com/catalog/services/natural-language-understanding) and create an instance.
   - Get your **API Key** and **URL** from the Watson NLU service credentials page.

4. **Set Up Environment Variables:**
   - Create a `.env` file in the root directory and add the following:
     ```
     WATSON_API_KEY=your_watson_api_key
     WATSON_API_URL=your_watson_api_url
     ```

5. **Run Flask Server:**
   ```bash
   python app.py
   ```

6. **Use ngrok (Optional for Web Deployment):**
   If you want to make your Flask app accessible over the web, you can use ngrok:
   ```bash
   ngrok http 5000
   ```
   Use the URL provided by ngrok to access the app externally.

### Running the Application 🏃

1. **Start the Flask Server:**
   ```bash
   python app.py
   ```
   The Flask app will be running on `http://localhost:5000`.

2. **Test Emotion Detection:**
   - Open your browser and go to `http://localhost:5000`.
   - Input some text and hit the **Submit** button.
   - The system will analyze the text and return the detected emotions, including their intensity.

3. **View Emotion Analysis:**
   The output will display a breakdown of the emotions detected in your input text, with percentages and a graphical representation of each emotion's intensity.

## Usage Example 🎬

### Example Input:
```
"I feel so happy today! Everything is going right and I can't stop smiling."
```

### Example Output:
```
Emotion Detected:
- Joy: 95%  
- Surprise: 5%
```

## License 📝

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements 🙏

- 🧠 [IBM Watson NLU](https://cloud.ibm.com/catalog/services/natural-language-understanding) for providing the AI capabilities for emotion detection.
- 🐍 [Flask](https://flask.palletsprojects.com/en/2.0.x/) for creating a simple web interface.
- 🎨 [Bootstrap](https://getbootstrap.com/) for easy frontend styling (optional).
- 🌍 [ngrok](https://ngrok.com/) for exposing the Flask app to the web (optional).

