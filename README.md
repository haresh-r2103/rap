# 📰 NewsBrief: AI-Powered News Summarizer Chatbot

**NewsBrief** is an interactive AI chatbot that fetches the latest news articles about companies or topics and summarizes them in multiple styles. Designed for clarity, simplicity, and accessibility, NewsBrief helps users quickly stay updated with concise news summaries—whether formal, friendly, or bullet-style.

---

## 🚀 Features

✅ Fetches the latest news from the web using DuckDuckGo  
✅ Extracts full article content using `trafilatura`  
✅ Summarizes news in multiple formats using Hugging Face Transformers  
✅ Built-in conversation interface with Gradio  
✅ Works on CPU (no GPU needed)  
✅ Handles casual conversation (greetings, small talk)  
✅ Easily extendable for different summarization models or formats

---

## 🎯 Use Case

Ideal for:
- Students and professionals who want quick updates
- Financial analysts or business enthusiasts tracking companies
- Anyone wanting AI-powered article summarization

---

## 🧠 How It Works

1. **User Input**  
   → e.g., "What's going on with Microsoft?"

2. **DuckDuckGo Search**  
   → Retrieves the latest article links relevant to the query.

3. **Content Extraction**  
   → `trafilatura` fetches clean text from article pages.

4. **Summarization**  
   → A transformer-based summarizer (like `facebook/bart-large-cnn`) condenses the text in one of the chosen formats:
   - Business Formal
   - Friendly Casual
   - Bullet Points
   - News Headlines

5. **Gradio UI**  
   → Displays the summarized news and supports a conversational chat interface.

---

## 🛠 Installation

Install the required Python packages:

```bash
pip install duckduckgo_search trafilatura transformers torch gradio
