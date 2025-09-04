
# 🧠 AI Study Buddy

**AI Study Buddy** is a smart Python assistant that helps students and self-learners study more efficiently by extracting, summarizing, and quizzing content from PDF textbooks or notes. It leverages NLP and Transformers to provide text summarization, flashcard generation, and question-answering capabilities—all in one CLI-based tool.

## 🚀 Features

- 📄 **PDF Reader**: Extracts text from PDF files.
- 📝 **Text Summarization**: Uses a T5 model to generate concise summaries.
- ❓ **Question Answering**: Ask questions about your study material and get instant answers.
- 🧾 **Flashcard Generator**: Creates basic flashcards based on named entities in the text.
- 🔊 **Optional TTS (Text-to-Speech)**: Reads responses aloud (disabled by default).

## 🛠️ Technologies Used

- Python 3
- [Transformers](https://huggingface.co/transformers/) (`t5-small`)
- PyPDF2
- spaCy (`en_core_web_sm`)
- pyttsx3 (for TTS)
- torch (PyTorch)

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/knightRehman/ai-study-buddy.git
   ```
   ```bash
   cd ai-study-buddy
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Or manually install:
   ```bash
   pip install transformers pyttsx3 spacy PyPDF2 torch
   ```

   ```bash
   python -m spacy download en_core_web_sm
   ```

4. (Optional for TTS):
   ```bash
   sudo apt-get install espeak
   ```

## 🧪 Usage

Run the script:

```bash
python ai_study_buddy.py
```

Follow the prompts to:

1. Enter your PDF path.
2. Choose from options:
   - Summarize the content
   - Ask a question
   - Generate flashcards
   - Exit

> Tip: Toggle TTS on/off by setting the `USE_TTS` variable at the top of the script.

## 🧠 Example

```
Options:
1. Summarize
2. Ask a question
3. Generate flashcards
4. Exit
```

## 📁 File Structure

```
ai-study-buddy/
├── ai_study_buddy.py
└── README.md
```

## ✨ Future Improvements

- GUI or Web interface (e.g. Streamlit)
- More intelligent flashcard generation
- Custom model support
- Persistent user session history

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

## 📄 License

MIT License
