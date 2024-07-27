
# YouTube Transcript Summarizer

This project provides a tool to summarize YouTube video transcripts. The tool includes a Flask web application and a Chrome extension to fetch and summarize YouTube transcripts.

## Prerequisites

1. **Anaconda** (for creating a virtual environment)
2. **Python** (version 3.6 or higher)
3. **Google Chrome** (for using the Chrome extension)

## Setup Instructions

### 1. Create a New Anaconda Virtual Environment

Open your terminal and create a new Anaconda virtual environment:

\`\`\`bash
conda create --name youtube_transcript python=3.8
\`\`\`

Activate the environment:

\`\`\`bash
conda activate youtube_transcript
\`\`\`

### 2. Clone the GitHub Repository

Open Visual Studio Code (VSCode), choose a folder, and clone the repository:

\`\`\`bash
git clone https://github.com/KalluSreevani/YouTube-Summarizer.git
\`\`\`

Navigate to the cloned directory:

\`\`\`bash
cd YouTube-Summarizer
\`\`\`

### 3. Install Dependencies

Ensure the \`Requirements.txt\` file is updated to use \`scikit-learn\` instead of \`sklearn\`.

Install the required packages:

\`\`\`bash
pip install -r Requirements.txt
pip install tensorflow
pip install tf-keras
pip install torch
\`\`\`

### 4. Download NLTK Data

Enter the Python shell from the terminal:

\`\`\`bash
python
\`\`\`

Import \`nltk\` and download the \`punkt\` package:

\`\`\`python
import nltk
nltk.download('punkt')
exit()
\`\`\`

### 5. Start the Flask Application

Run the Flask application:

\`\`\`bash
python TranscriptApp.py
\`\`\`

This will start a local server at \`http://127.0.0.1:5000/\`. Ignore any errors and proceed to the next steps.

### 6. Load the Chrome Extension

1. Open Google Chrome and go to \`chrome://extensions/\`.
2. Enable the Developer mode toggle in the top right corner.
3. Click on \`Load unpacked\` and select the directory where you cloned this repository (e.g., \`C:\Users\jadha\OneDrive\Desktop\Youtube_transcript\YouTube-Summarizer\extension\`).
4. Pin the extension in the Chrome toolbar.

### 7. Using the Extension

1. Go to YouTube.
2. Click on the pinned extension icon.
3. Click on "Summarize" to fetch and summarize the transcript of the currently opened YouTube video.

## Important Dependencies

- \`flask >= 2.3.2\`
- \`youtube_transcript_api >= 0.6.1\`
- \`transformers >= 4.30.2\`
- \`sentencepiece >= 0.1.99\`
- \`scikit-learn\`
- \`langdetect >= 1.0.9\`
- \`nltk >= 3.8.1\`
- \`numpy >= 1.23.3\`

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

