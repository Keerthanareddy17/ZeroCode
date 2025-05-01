# ZeroCode - Prompt to UI Code Generator 🎨

ZeroCode is a powerful, local, and privacy-centric web application that converts voice or text prompts into deployable frontend code. Inspired by the CanvaCode concept, it allows users to describe their desired UI by either typing or speaking, and generates production-ready HTML, CSS, and JavaScript code. 🚀

## Features ✨

- **Voice Input 🎙️**: Users can describe their UI requirements by simply uploading a voice recording (in `.wav` format), which will be transcribed using Whisper for processing.
- **Text Input 📝**: Alternatively, users can type their UI requirements directly into a text box.
- **Code Generation 💻**: The app utilizes Groq's LLaMA model to generate HTML/CSS code based on the given prompt.
- **UI Preview 👀**: After generating the code, users can preview the UI directly on the dashboard.
- **Code Download 📦**: Users can download the generated frontend code as a zip file, which includes an HTML file ready for deployment.

## Project Structure 🗂️

Here's a brief overview of the key files and directories in the project:

- **`app.py`**: The main application file where the Streamlit dashboard is created, including the functionality for voice and text inputs, code generation, and preview.
- **`transcriber.py`**: Handles audio transcription using Whisper to convert voice recordings into text prompts.
- **`codegen.py`**: This file contains the logic to generate frontend code using the LLaMA model (Groq) based on the user’s input.
- **`static/`**: Directory for storing any static assets like images or CSS files if required in the future.
- **`requirements.txt`**: List of Python dependencies needed to run the project.

## Prerequisites ⚙️

Before running the project, you need to have the following installed:

- Python 3.8 or higher 🐍
- A text editor (e.g., VSCode or Sublime Text) for editing the code
- [Groq API Key 🔑](https://groq.com/) (for code generation)

## Step-by-Step Setup Guide 🛠️

### 1. **Create a Virtual Environment** 🌱

#### On Mac or Linux:
1. Open your terminal.
2. Navigate to your project directory.
3. Run the following commands to create and activate a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
```
#### On Windows:
1. Open Command Prompt or PowerShell.
2. Navigate to your project directory.
3. Run the following commands to create and activate a virtual environment:
```
python -m venv venv
.\venv\Scripts\activate
```

### 2. Install Dependencies 📦

Once your virtual environment is activated, install the required Python packages by running:

```
pip install -r requirements.txt
```
This will install all the dependencies mentioned in requirements.txt.

### 3. Set Up Groq API 🔑

1. Create a Groq account if you don’t have one.
2. After logging in, generate an API key from the Groq dashboard.
3. Create a .env file in the project root directory and add your Groq API key like so:

```
GROQ_API_KEY=your_groq_api_key
```
### 4. Running the App ▶️

After installing dependencies and setting up the API key, you can run the app with the following command:
```
streamlit run app.py
```
This will start the Streamlit web app. The application will be accessible in your browser. 🌐

### 5. Using the Application 💡

Once the app is running:

1. Text Prompt 📝: Enter your desired UI description (e.g., "A simple login page with a header") in the text box and click "✨ Generate UI Code".
2. Voice Input 🎙️: Upload a .wav file with your voice prompt, click "🚀 Transcribe Voice Prompt", and once transcribed, click "✨ Generate UI Code".
3. Preview 👀: After the UI code is generated, you can preview it directly in the "🔍 Preview Your UI" section.
4. Download Code 📦: Click the "📁 Download Code" button to download a zip file containing the generated code.

Feel free to reach out for collaboration, feedback, or just to say hi! 👋
- 📧 Email: katasanikeerthanareddy@gmail.com
- 💼 LinkedIn: [https://www.linkedin.com/in/keerthana-reddy-katasani-b07238268/]


