## Requirements 

python3.6

## Commands to Run on Linux
### Create virtual environment
```
python3.6 -m venv venv 
```
### To activate the virtual environment
```
source ./venv/bin/activate 
```
### Install all required python libraries
```
pip install -r requirements.txt 
```
### Download all nltk_data to venv 
```
sudo python -m nltk.downloader -d ./venv/nltk_data all
```
### To to deactivate the virtual environment
```
deactivate
```

## Classification Of Methods

### TF-IDF
* Simple document vectors that represent how important a word is to a document within a corpus
* No consideration of context in which a word is used
* Creates very sparse,large vectors

### word2vec
* Word vectors created through a shallow, two-layer neural network; word vectors can then be averaged or summed to create document level vectors
* Creates smaller, dense vectors
* Word vectors do have context built in 

### doc2vec
* Document vectors created through a shallow, two-layer neural network
* Creates smaller, dense vectors
* Document vectors do have context built in

### Recurrent Neural Network
* A type of neural network that has an understanding of the data's sequential nature (forms a sense of memory)
* Dense vectors are created within the model


## Summary
* TF-IDF is quick and easy way to set a baseline
* Information is lost when averaging or summing word vectors
* doc2vec is slower but better than word2vec for sentence vectors
* RNN is extremely powerful even with limited data

