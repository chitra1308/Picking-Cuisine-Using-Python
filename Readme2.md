# ALGORITHM USED:
 
# Join():
The join() method provides a flexible way to concatenate string. It concatenates each element
of an iterable (such as list, string and tuple) to the string and returns the concatenated string.
The syntax of join() is:
string.join(iterable)

# Strip():
The strip() removes characters from both left and right based on the argument (a string specifying the set of characters to be removed). This method was implemented to train data and test data set to create “Clean String”
The syntax of strip() is:
string.strip([chars])

# Wordnet lemmatizer:
Stemming and Lemmatization are the basic text processing methods for English text. The goal of both stemming and lemmatization is to reduce inflectional forms and sometimes derivationally related forms of a word to a common base form. 
Lemmitize:
Lemmatization is the process of grouping together the different inflected forms of a word so they can be analysed as a single item. Lemmatization is similar to stemming but it brings context to the words. So it links words with similar meaning to one word.
 
# NLTK Corpus:
The nltk.corpus package automatically creates a set of corpus reader instances that can be used to access the corpora in the NLTK data package

# Vectorizer:
Bag-of-Words is a very intuitive approach to this problem, the methods comprise of:
•	Splitting the documents into tokens by following some sort of pattern.
•	Assigning a weight to each token proportional to the frequency with which it shows up in the document and/or corpora.
•	Creating a document-term matrix with each row representing a document and each column addressing a token.
Vectorizer.fit_transform():
Convert a collection of text documents to a matrix of token counts.
tfidfvectorizer.transform:
transform method accepts a corpus, so for a single document, you should pass it as list, or it is treated as iterable of symbols, each symbol being a document.

# LinearSVC:
Linear Support Vector Classification.
Similar to SVC with parameter kernel=’linear’, but implemented in terms of liblinear rather than libsvm, so it has more flexibility in the choice of penalties and loss functions and should scale better to large numbers of samples.
This class supports both dense and sparse input and the multiclass support is handled according to a one-vs-the-rest scheme.
 
# Classifier.fit(Predictors_tr,targets_tr);
Build a forest of trees from the training set (X, y).
Fit(X,y,sample_weight=none)
X : array-like or sparse matrix of shape = [n_samples, n_features]
The training input samples. Internally, its dtype will be converted to dtype=np.float32. If a sparse matrix is provided, it will be converted into a sparse csc_matrix.
y : array-like, shape = [n_samples] or [n_samples, n_outputs]
The target values (class labels in classification, real numbers in regression).
sample_weight : array-like, shape = [n_samples] or None
Sample weights. If None, then samples are equally weighted. Splits that would create child nodes with net zero or negative weight are ignored while searching for a split in each node. In the case of classification, splits are also ignored if they would result in any single class carrying a negative weight in either child node.

# Classifier.Predict(Predictors_ts):
Predict(X):
Predict class for X.
The predicted class of an input sample is a vote by the trees in the forest, weighted by their probability estimates. That is, the predicted class is the one with highest mean probability estimate across the trees.
Parameters:
X : array-like or sparse matrix of shape = [n_samples, n_features]
The input samples. Internally, its dtype will be converted to dtype=np.float32. If a sparse matrix is provided, it will be converted into a sparse csr_matrix.
Returns:
y : array of shape = [n_samples] or [n_samples, n_outputs]
The predicted classes.

