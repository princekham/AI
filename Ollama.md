### Installation

```
curl -fsSL https://ollama.com/install.sh | sh
```
### pulling models

```
# Pull the lightweight chat model
ollama pull qwen2.5:1.5b
```
-For multilingual retrieval involving Burmese and English, use Nomic's multilingual model variant instead:

```
ollama pull nomic-embed-text-v2-moe
```

- I had to use http://127.0.0.1:11434 to connect to ollama from n8n when creating credential
