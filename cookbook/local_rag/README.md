## Fully Local RAG using Ollama & PgVector

> Note: Fork and clone this repository if needed

1. [Install](https://github.com/ollama/ollama?tab=readme-ov-file#macos) and run ollama

```shell
ollama run openhermes
```

2. Create a virtual environment

```shell
python3 -m venv ~/.venvs/aienv
source ~/.venvs/aienv/bin/activate
```

3. Install libraries

```shell
pip install -r cookbook/local_rag/requirements.txt
```

4. Run pgvector

```shell
phi start cookbook/local_rag/resources.py -y
```

5. Run CLI application

```shell
python cookbook/local_rag/cli.py
```

- Ask questions about thai recipes

```text
Got any pad thai?
```

6. Run Streamlit application

```shell
python cookbook/local_rag/app.py
```

- Upload you own PDFs and as

7. Turn off pgvector

```shell
phi stop cookbook/local_rag/resources.py -y
```

8. Message me on [discord](https://discord.gg/4MtYHHrgA8) if you have any questions

9. Star ⭐️ the project if you like it.