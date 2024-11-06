# AI and RAG; chat with documents

The accompanying presentation is available as "ResBaz2024-AIandRAG.pdf" in this folder, and [online](https://docs.google.com/presentation/d/1fCUuci69uKic0I6uHIq3C2OSNNM8I30K-0BGWR6su3g/edit?usp=sharing). 

## Things you'll need
- A Gemini API key (requires Google Account): [aistudio.google.com](https://aistudio.google.com/app/apikey)
- Jupyter installed `pip install jupyter`
- Some reference documents to perform rag over (see the list of open access documents below if you need ideas!)

### Open access papers (that can be used as a sample document collection)
- https://ora.ox.ac.uk/objects/uuid:874607b1-b700-45a7-8877-19df4b889fce/files/rd791sg46t
- https://bmcmedicine.biomedcentral.com/counter/pdf/10.1186/s12916-019-1377-7.pdf
- https://journals.sagepub.com/doi/pdf/10.1177/2056305118763366
- https://www.altex.org/index.php/altex/article/download/2607/2552/24817
- https://www.sciencedirect.com/science/article/pii/S037872061400007X

## Getting started
The following are all executed from the command line or terminal

Create a new virtual environment and activate it
```
python3 -m venv .venv
source .venv/bin/activate           # Linux/MacOS
source .venv\Scripts\activate       # Windows
```

Install the project requirements
```
pip install -r requirements.txt
```

Add your Gemini API key to the .env file (replace "MY-API-KEY-HERE" with your key)
```
# Linux
echo 'GEMINI_API_KEY="MY-API-KEY-HERE"' >> .env

# Windows
echo GEMINI_API_KEY="MY-API-KEY-HERE"> .env
```

Start the Jupyter server
```
jupyter notebook
```

## The workbooks

#### Interacting-with-Gemini.ipynb
Shows basic initialisation of Gemini and making calls to the Gemini API using Google's generativeai python module

#### RAG-with-Gemini.ipynb
Shows how to generate embeddings, and use them in a RAG pipeline centered around Gemini

#### RAG-with-Gemini-workshop.ipynb
The working copy of RAG-with-Gemini.ipynb, used for demonstration purposes.


