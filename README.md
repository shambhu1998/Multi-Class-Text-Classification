# Multi-Class-Text-Classification
Used two methods for classifying the text sequences into respective categories:<br>
**1. ML Algorithms**<br>
**Steps:**<br>
* First, Tfidf vectorizer will tokenize the documents, learn vocabulory, inverse document frequency weightings and allow us to encode new document. Then, this ecoded data is passed for classification.<br>
* Used different machine learning algorithms like Naive Bayes, SVM, Logistic Regression and Random Forest.
* Trained each model and compared results 
* Picked the best model and analyzed the result.

**2. LSTM Model**<br>
Since the most of the data contains random combination of characters and words rather than proper word in dictionary, it seems to be best to use character based LSTM model rather than word based. So, I've used character based lstm model and trained it using pytorch.<br>
**Steps:**<br>
* First, create the custom dataset class to generate dataset.
* After creating dataset, it uses this dataset to generate data loader by using Pytorch's DataLoader method which gives the iterable over the dataset.
* Define the LSTM model architecture using Pytorch's nn.Module 
* Train and evaluate the model over predefined number of epochs.
* Finally, Analyze the results.

I've trained the lstm model by changing different hyper-parameters in lstm architecture like number of hidden states, directionality, regularization, etc. and able to get a  descent validation accuracy.<br>

I have not tried using transformer architecture or pretrained models like BERT as the dataset is small and contains random words or combination of characters. 


