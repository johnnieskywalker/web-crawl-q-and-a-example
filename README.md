# Web  Q&A with Embeddings (forked from openai tutorial)

Learn how to crawl your website and build a Q/A bot with the OpenAI API. You can find the full tutorial in the [OpenAI documentation](https://platform.openai.com/docs/tutorials/web-qa-embeddings).

[Original repo](https://github.com/openai/web-crawl-q-and-a-example)

# Buidl

To build the project, you need to install the dependencies:

```bash
python -m venv env

source env/bin/activate

pip install -r requirements.txt
```

# Please use your own API key in .env file

.env example:

```bash
OPENAI_API_KEY=your-api-key
```

# About the project
The web-qa.py script is a modified version of an OpenAI tutorial that demonstrates how to build a question-answering bot using the OpenAI API. This version of the script is specifically designed to answer questions about Ethna, a project in the Ethereum ecosystem. It does this by crawling the Ethna documentation, extracting the text, and using the OpenAI API to generate embeddings for the text. These embeddings are then used to find the most similar context to a given question, which is then used to generate an answer.

The processed files, which include the extracted text and the generated embeddings, are included in the repository. This makes the repository quite large, but it also saves some OpenAI API calls, as the embeddings don't need to be generated every time the script is run. This is particularly useful for learning and experimentation, as it allows you to explore the data and the embeddings without incurring additional API costs.

Please note that this project is just for fun and learning. It's not intended to be a production-ready solution, but rather a starting point for learning about the OpenAI API and how it can be used to build question-answering bots.
