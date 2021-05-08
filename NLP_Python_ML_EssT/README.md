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
