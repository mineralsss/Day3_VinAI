# Lab 3: Chatbot vs ReAct Agent (Industry Edition)

Welcome to Phase 3 of the Agentic AI course! This lab focuses on moving from a simple LLM Chatbot to a sophisticated **ReAct Agent** with industry-standard monitoring.

## 🚀 Getting Started

### 1. Setup Environment
Copy the `env_example.txt` to `.env` and fill in your API keys:
```bash
cp .env.example .env
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

## 🏠 Running with Local Models (CPU)

If you don't want to use OpenAI or Gemini, you can run open-source models (like Phi-3) directly on your CPU using `llama-cpp-python`.

### 1. Download the Model
Download the **gemma-4-E4B-it-GGUF** (approx 5.07GB) from Hugging Face:
- [unsloth/gemma-4-E4B-it-GGUF](https://huggingface.co/unsloth/gemma-4-E4B-it-GGUF/blob/main/gemma-4-E4B-it-Q4_1.gguf)

### 2. Place Model in Project
Create a `models/` folder in the root and move the downloaded `.gguf` file there.


### 3. Get your Serpapi key
Go to [Link](https://serpapi.com) and get your own api key in order for some tools to work
then place api key in `.env` 

### 3. Update `.env`
Change your `DEFAULT_PROVIDER` and set the path:
```env
DEFAULT_PROVIDER=local
LOCAL_MODEL_PATH=./models/gemma-4-E4B-it-Q4_1.gguf
```
Go to [Quick Start](./QUICKSTART.md) for more information


*Happy Coding! Let's build agents that actually work.*
