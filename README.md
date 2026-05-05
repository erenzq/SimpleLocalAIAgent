# Pizza Review QA (LangChain + Ollama)

This project is a simple **question-answering system** for restaurant (pizza) reviews using **LangChain** and locally running **Ollama models**.

## What does it do?

* Loads a CSV file with restaurant reviews
* Converts the reviews into **embeddings (vectors)**
* Stores them in a local vector database (Chroma)
* Retrieves the most relevant reviews for a given question
* Uses an LLM to generate an answer based on those reviews

---

## Use your own data

You can easily plug in your own CSV file.

The CSV should have roughly this structure:

* `Title`
* `Review`
* `Rating`
* `Date`

Example:

```
Title,Review,Rating,Date
Great Pizza,Best pizza ever!,5,2024-01-01
```

---

## Installation

1. Install dependencies:

```
pip install -r requirements.txt
```

2. Run Ollama and download the models:

```
ollama pull llama3.2
ollama pull mxbai-embed-large
```

---

## Usage

Start the program:

```
python main.py
```

Then ask questions like:

* "Is the pizza good?"
* "What do customers say about the service?"

---

