# Nova AI — Voice Command Assistant

Nova AI is a web-based voice assistant built with **Python Flask and Web Speech API**. It processes voice commands to perform actions such as YouTube searches and Gmail email drafting.

## Features

* Voice command recognition
* Voice-based command processing
* YouTube search and playback
* Gmail email drafting
* Modern animated user interface
* Web-based application
* Responsive design
* Deployable on Render

## Technologies Used

* **Python**
* **Flask**
* **HTML5**
* **CSS3**
* **JavaScript**
* **Web Speech API**
* **YouTube**
* **Gmail**
* **Gunicorn**
* **Render**

## How It Works

1. Click the microphone button.
2. Speak a command.
3. The browser converts speech into text using the Web Speech API.
4. The command is sent to the Flask backend.
5. Nova AI processes the command.
6. The required action is opened in a new browser tab.

## Example Commands

### YouTube

```text
Open YouTube and play Karuppu song
```

```text
Play Aasa Kooda on YouTube
```

```text
Open YouTube and play Shape of You
```

### Gmail

```text
Email john at gmail.com type hello
```

```text
Gmail john at gmail.com write meeting tomorrow
```

The Gmail feature prepares an email draft with the recipient and message content.

## Project Structure

```text
nova-ai/
│
├── app.py
├── requirements.txt
├── README.md
│
└── templates/
    └── index.html
```

### `app.py`

Contains the Flask backend, voice command processing, YouTube search, and Gmail URL generation.

### `index.html`

Contains the frontend interface, microphone button, animations, voice recognition, and communication with the Flask backend.

### `requirements.txt`

Contains the Python packages required to run the project.

## Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/nova-ai.git
cd nova-ai
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the application

```bash
python app.py
```

Open your browser and visit:

```text
http://127.0.0.1:8000
```

## Deployment

Nova AI can be deployed on **Render** using Gunicorn.

### Build Command

```bash
pip install -r requirements.txt
```

### Start Command

```bash
gunicorn app:app
```

## Privacy

Nova AI does not require users to provide passwords or API keys.

Microphone access is handled by the browser's Web Speech API. Browser microphone permission may be required for voice recognition.

## Limitations

* Voice recognition depends on browser support.
* Internet connection is required for online services.
* YouTube search depends on the YouTube results page.
* Gmail functionality creates an email draft rather than sending the email automatically.
* The current version supports a limited number of voice commands.

## Future Improvements

* Integration with AI/LLM models
* Text-to-speech responses
* Google Search commands
* Google Calendar integration
* More application integrations
* Multi-language voice recognition
* Advanced natural-language command processing
* Command history
* Secure OAuth authentication

If you like this project, consider giving the repository a star!
