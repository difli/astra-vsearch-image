# astra-vsearch-image
Jupyter notebook for image search powered by [Astra Vector Search](https://docs.datastax.com/en/astra-serverless/docs/vector-search/overview.html) and OpenAI [CLIP Model](https://github.com/openai/CLIP).

## OpenAI CLIP Model
CLIP, or "Contrastive Language-Image Pretraining", is an artificial intelligence model developed by OpenAI. The model is trained to understand and associate images with natural language by using a vast number of images and their associated textual descriptions. CLIP can perform tasks such as generating textual descriptions of images or finding images based on given text.

## Astra Vector Search
Astra vector search enables developers to search a database by context or meaning rather than keywords or literal values. This is done by using “embeddings”. Embeddings are a type of representation used in machine learning where high-dimensional or complex data is mapped onto vectors in a lower-dimensional space. These vectors capture the semantic properties of the input data, meaning that similar data points have similar embeddings. The CLIP model is used to generate the embeddings in this demo.

## Demo Summary
- The CLIP model generates embeddings for each image 
- Metdata and embeddings for each image are stored in Astra DB. 
- The embeddings are stored in a Astra DB column of Type Vector.  
- The idea of the demo is to find with the help of Astra Vector Search the image of the house with a swimming pool.
- The CLIP model generates embeddings based on the search string: "a house with a swimming pool". 
- This embedding is used in the query to find the image that has similar embeddings as the search string.
- You should see the image of a house with a swimming pool
