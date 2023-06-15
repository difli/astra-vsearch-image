# astra-vsearch-image
Jupyter notebook for image search powered by [Astra Vector Search](https://docs.datastax.com/en/astra-serverless/docs/vector-search/overview.html) and OpenAI [CLIP Model](https://github.com/openai/CLIP).

## OpenAI CLIP Model
CLIP, or "Contrastive Language-Image Pretraining", is an artificial intelligence model developed by OpenAI. The model is trained to understand and associate images with natural language by using a vast number of images and their associated textual descriptions. CLIP can perform tasks such as generating textual descriptions of images or finding images based on given text.

## Astra Vector Search
Astra vector search enables developers to search a database by context or meaning rather than keywords or literal values. This is done by using “embeddings”. Embeddings are a type of representation used in machine learning where high-dimensional or complex data is mapped onto vectors in a lower-dimensional space. These vectors capture the semantic properties of the input data, meaning that similar data points have similar embeddings. 

## Demo Summary
The demo showcases the CLIP model, which generates embeddings for images. These embeddings, along with metadata, are stored in Astra DB. Specifically, the embeddings are stored in a column of type Vector. The goal of the demo is to utilize Astra Vector Search to find an image of a house with a swimming pool. The CLIP model generates embeddings based on the search string "a house with a swimming pool". These embeddings are then used in a query to find an image that shares similar embeddings with the search string, ultimately displaying an image of a house with a swimming pool.
