# AI Article Summarizer

## Overview

AI Article Summarizer is a Chrome Extension built using Manifest V3 that leverages the Gemini API to generate intelligent summaries from web articles in real time. The extension extracts textual content directly from active webpages and provides users with multiple summarization formats, including concise summaries, detailed explanations, and structured bullet points.

The project demonstrates practical implementation of browser extension development, DOM manipulation, asynchronous API integration, and modern client-side application architecture.

---

## Features

* AI-powered article summarization using Gemini 2.5 Flash
* Real-time extraction of webpage content
* Multiple summarization modes:

  * Brief Summary
  * Detailed Summary
  * Bullet Point Summary
* Secure API key management using Chrome Storage API
* One-click copy to clipboard functionality
* Responsive and minimal user interface
* Chrome Manifest V3 compliant architecture

---

## Technology Stack

| Category       | Technologies                  |
| -------------- | ----------------------------- |
| Frontend       | HTML5, CSS3, JavaScript (ES6) |
| Browser APIs   | Chrome Extension APIs         |
| AI Integration | Gemini 2.5 Flash API          |
| Storage        | Chrome Storage Sync API       |
| Architecture   | Manifest V3                   |

---

## System Architecture

```bash
AI-Article-Summarizer/
│
├── manifest.json
├── popup.html
├── popup.js
├── content.js
├── background.js
├── options.html
├── options.js
└── icon.png
```

---

## Core Functionality

### Content Extraction

The extension extracts article content dynamically from active webpages using DOM traversal techniques. It prioritizes semantic `<article>` elements and falls back to paragraph aggregation when necessary. 

### AI-Based Summarization

Extracted content is processed using Gemini API prompts tailored to the selected summarization mode. The system supports concise summaries, detailed explanations, and structured bullet-point outputs. 

### Secure Configuration Management

User API credentials are securely stored using Chrome synchronized storage, ensuring persistence across sessions while maintaining local privacy. 

### Interactive User Interface

The extension provides a responsive popup interface for summary generation, content visualization, and clipboard operations. 

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/ai-article-summarizer.git
cd ai-article-summarizer
```

### Load Extension in Chrome

1. Open Chrome and navigate to:

```bash
chrome://extensions/
```

2. Enable **Developer Mode**
3. Select **Load Unpacked**
4. Choose the project directory

---

## Gemini API Configuration

1. Generate an API key from Google AI Studio
2. Open the extension settings page
3. Enter the Gemini API key
4. Save the configuration

The extension automatically redirects users to the settings page if no API key is detected during installation. 

---

## Performance Highlights

* Implemented dynamic DOM-based article extraction for real-time summarization workflows
* Designed asynchronous API request handling for optimized user interaction
* Integrated secure browser-based credential management using Chrome Storage APIs
* Developed a scalable Manifest V3 extension architecture aligned with modern Chrome standards

---

## Future Enhancements

* Multi-language summarization support
* PDF and document summarization
* AI-powered contextual insights
* Cloud synchronization
* Export summaries to PDF or Markdown
* Reading analytics dashboard

---

## License

This project is licensed under the MIT License.

---

## Author

Developed as a modern AI-powered browser productivity solution using JavaScript, Chrome APIs, and Gemini AI.
