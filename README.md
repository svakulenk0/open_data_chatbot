# Open Data (OD) Chatbot

## Setup

1) install requirements

pip install -r requirements.txt  

2) download spacy english model

python -m spacy download en  

3) train NLU and CORE

python trainer.py train-all-s  


## Run

1) run actions server

python -m rasa_core_sdk.endpoint -p 5002 --actions actions

2) run http server from webchat folder

python -m http.server 80

3) run webchat

python run_webchat.py

4) chatbot is running at http://localhost/index.html
