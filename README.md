# ClusteringOnPubmed
This project performs the document clustering task and classification task of SVM using an archived medline document set.

After retrieving the data from an archived pubmed document, it is preprocessed with: stemming, tokenization, punctuation removal, int normalization, and stopword removal. After the data is cleaned, it is then put into a list of documents and a vocab counter. After all of the documents are inserted, all of the empty documents are removed, and unique words are removed from the vocab in order to help the accuracy. 

After the ddata is processed, the number of documents per cluster is printed, then the data is visualized with pyLDAvis. The labels are chosen for each document next. I then used Train test split to create a training and testing dataset with a 90/10 split. After this, a pipeline was created to verctorize the documents. Lastly, the data was fit to the model, and the accuracy was evaluated with the built in scoring function. 


-PubmedClustering.py contains all the source code to run the model. 

-trained-mdl.pkg contains all of my preprocessed data.

-clusters-vis.html contains the pyLDAvis model that was created.

-pubmed21n0009.xml contains the original pubmed data file.

This implementation of GSDMM is from https://github.com/rwalk/gsdmm/tree/master/gsdmm
