# Retrieval evaluation with query expansion



### Built on the retrieval_evaluation repository. Consult the [readme](https://github.com/michaelprem/retrieval_evaluation/blob/master/README.md) of that repository for prerequisites.

### In addition (pip) install:  (if not installed already):

- pyenchant - a dictionary to consult for finding "real" English words, 
- wget for dowloading model files from the internet
- bz2 for decompressing compressed file
- shutil for saving decompressed files.
- gensim for word2vec models

The repository tests two types of query expansion:

- expand_wn(): based om wordnet synomyms (using the NLTK package)
- expand_w2v() based on embeddings: word2vec models (using the gensim package and downloaded embeddings). This takes about 15-20 minutes of file downloading and model loading first time a model is used, but repeated tests can be done on a loaded model. 


