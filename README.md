# Open Data (OD) Chatbot

## Setup

* install requirements

pip install -r requirements.txt  

* download spacy english model

python -m spacy download en  

* train NLU and CORE

python trainer.py train-all-s  


## Run

2) 

1) run actions server

python -m rasa_core_sdk.endpoint -p 5002 --actions actions

3) run http server from webchat folder

python -m http.server 80

4) run webchat

python run_webchat.py

5) chatbot is running at http://localhost/index.html
