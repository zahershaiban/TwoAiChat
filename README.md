

# 🦙🤖 LLaMA × GPT-4o-mini

A simple **two-agent conversation** between **LLaMA 3 (8B Instruct)** and **GPT-4o-mini**.

Each model has its own personality and takes turns responding by **replaying the full conversation history** every time.

---

## How it works

* LLaMA runs via **Hugging Face (OpenAI-compatible API)**
* GPT-4o-mini runs via **OpenAI**
* Each model:

  * sees itself as `assistant`
  * sees the other as `user`
* Memory is handled manually by rebuilding message history

---

## Personalities

* **LLaMA** → optimistic, positive, casual
* **GPT-4o-mini** → pessimistic, skeptical, casual

Responses are short and informal.

---

## Setup in .env

```bash
HF_TOKEN=hf_...
OPENAI_API_KEY=sk-...
```

Run the script and watch the models talk.

