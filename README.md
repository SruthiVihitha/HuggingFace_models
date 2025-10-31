# 🤖 AI/NLP/VQA Project Gallery

This repository showcases four projects demonstrating state-of-the-art Generative AI, Computer Vision (VQA), and NLP tasks using Python libraries such as `transformers`, `google-generativeai`, `pyttsx3`, and `SpeechRecognition`.

## ⚙️ Setup and Installation

### 1. Prerequisites

- **Python 3.8+** is required.
- For the Talking Doctor GUI, ensure you have a working microphone and system-level **PortAudio** installed.

### 2. Dependencies

Install all libraries with `pip`:

```bash
pip install transformers torch requests Pillow google-generativeai pyttsx3 SpeechRecognition pyaudio
```

### 3. API Key Configuration

The Gemini-based Talking Doctor needs a Google Gemini API Key.

- Obtain the API key from Google AI Studio.
- Set your key as an environment variable for security ():
  - **Windows (Powershell):**
    ```powershell
    $env:GEMINI_API_KEY="YOUR_API_KEY"
    ```
  - **Linux/macOS:**
    ```bash
    export GEMINI_API_KEY="YOUR_API_KEY"
    ```
- You can directly hardcode it in `talking_doctor.py` (not recommended for production) or update the script to use the environment variable for better security.

## 🚀 Project Demonstrations

### 1. Visual Question Answering (VQA)

**Code snippet:** See VQA block above.

| Detail           | Description                                                                            |
|:-----------------|:---------------------------------------------------------------------------------------|
| Model            | Salesforce/blip-vqa-capfilt-large                                                      |
| Task             | Answers a natural-language question about an input image                               |
| Example Input    | URL of a dogs photo                                                                    |
| Example Question | "what is the breed of the dogs?"                                                       |
| Output           | E.g., "golden retriever", "dogs"                                                       |

### 2. Abstractive Text Summarization

**Code snippet:** See summarizer block above.

| Detail       | Description                                                                    |
|:-------------|:-------------------------------------------------------------------------------|
| Model        | facebook/bart-large-cnn                                                        |
| Task         | Summarizes long articles into concise readable text                            |
| Example Input| Article about Liana Barrientos’s marriages                                     |
| Parameters   | max_length=130, min_length=30                                                  |
| Output       | Brief summary on marriage and legal issues                                     |

### 3. Masked Language Modeling (Fill-Mask)

**Code snippet:** See fill-mask block above.

| Detail       | Description                                                         |
|:-------------|:--------------------------------------------------------------------|
| Model        | distilbert-base-uncased                                             |
| Task         | Predicts a missing word ([MASK]) in sentences                       |
| Example Input| "ai is very [MASK] for mankind"                                     |
| Output       | Probable words: beneficial, important, useful, good, great          |

### 4. Interactive Talking Doctor Chatbot (Generative AI)

**File:** `talking_doctor.py`

| Detail        | Description                                                                                  |
|:--------------|:---------------------------------------------------------------------------------------------|
| Model         | gemini-1.5-flash                                                                             |
| Functionality | Tkinter desktop app with voice-to-text, Gemini dialogue, and text-to-speech                  |
| User Flow     | Click “Talk now”, speak, get a reply, and hear a spoken answer                              |
| Note          | Requires a microphone, all listed dependencies, and local doctor image as `download.jpg`     |

## ▶️ Video Demonstrations

Upload your project demos here!

| Project Name                 |   Status         | Description                                                        |
|:----------------------------|:----------------------------|:-------------------------------------------------------------------|
| Visual Question Answering    |  <img width="882" height="454" alt="image" src="https://github.com/user-attachments/assets/0c2ad91b-417b-4c8e-aa38-b57bc56c8e96" />
<img width="1169" height="877" alt="image" src="https://github.com/user-attachments/assets/dffc758e-5bd0-4258-b5ef-77d9007aabd7" />
    | Shows question answering on the dogs photo                          |
| Text Summarization          |    <img width="1690" height="689" alt="image" src="https://github.com/user-attachments/assets/3a631d08-6fb3-49fb-9a81-42b6779ae7d4" /><img width="1681" height="297" alt="image" src="https://github.com/user-attachments/assets/31943fce-e712-47b4-9884-f0f2c6d5afbd" />
| Demonstrates summarizer’s output                                   |
| Masked Language Modeling    | <img width="812" height="603" alt="image" src="https://github.com/user-attachments/assets/9a4f9abe-7424-429d-bc14-4ca7b211e9d4" />
 | Shows predicted words for `[MASK]`                                 |
| Talking Doctor Chatbot      |  "C:\Users\sruth\OneDrive\Desktop\projects\vids_aimer\talking_doc.mp4" | GUI, speech recognition, Gemini response, and text-to-speech demo  |

Visual Question Answering , Text Summarization , Masked Language Modeling 
"C:\Users\sruth\OneDrive\Desktop\projects\vids_aimer\VQA_MASK_S.mp4"
