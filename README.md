# Retrieval evaluation with query expansion

Michael Preminger

### Built on the retrieval_evaluation repository. Consult the [readme](https://github.com/michaelprem/retrieval_evaluation/blob/master/README.md) of that repository for prerequisites.

### In addition (pip) install:  (if not installed already):

- pyenchant - a dictionary to consult for finding "real" English words, 
- wget for dowloading model files from the internet
- bz2 for decompressing compressed file (probably available on system)
- shutil for saving decompressed files.
- gensim for word2vec models

The repository tests two types of query expansion:

- (function **expand_wn**()): based om wordnet synomyms (using the NLTK package)
- (function **expand_w2v**()) based on embeddings: word2vec models (using the gensim package and downloaded embeddings). This requires 3.5GB of free space, and  takes about 15-20 minutes of file downloading and model loading first time a model is used, but repeated tests can be done on a loaded model. 


