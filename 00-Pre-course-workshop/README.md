# Pre-course workshops
In this pre-course workshops was mentioned two main ideas. The first was RAG and the second was search engines. In RAG section I used elasticsearch and OpenAI API to build some simple RAG application. Also I built straightforward user interface with Streamlit. In the search engines section I mainly user scikit-learn, Pytorch and Transfomers library.

## RAG
The main goal of this pre-course was to build simple RAG on the Q&A from the Zoomcamp different courses. The data was stored in json format. First I loaded data and established connection with elasticsearch (before that I had to run docker image with elastic search). Next step was to indexing documents and retrieve data with Elasticsearch. The last phase was to create prompt template and boost the LLM answers with some context, then all code was turned into function. To built user interface I created two python scripts: app.py and rag.py. In summary I learned about RAG and how easily it can be implemented with Q&A data and OpenAI API. Below you can see the user interface:

![Zrzut ekranu 2024-06-25 223828](https://github.com/KacperUrban/llm-zoomcamp/assets/87485442/b064b6a8-e432-40df-86ec-33df13c36496)


## Search engines
The main objective of this pre-course was to get more knowledge about search engines, embedings etc. So on the begining I loaded data and then i did basic text search. First was a keyword filtering. We can filter some data for example in dataframe on particular keyword. Second type was based on data vectorization. The first method was a bag of words (in sklearn is implemented by CountVectorizer). This approach is really simple, we can decode each document with counting every word in this document. The second method was a TF-IDF (term frequency - inverse document frequency). This method is a little bit more complex, but still intuitive. Then to calculate a similiarty score was used dot product and cosine similarty. In the next step I dive into creating simple embedding with SVD and NMF. The last step was to use BERT to create embedding.
