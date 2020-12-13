# NLP_final_project

NLP final project. Create a doctor chatbot that carries out conversation regarding COVID-19

### Set up the virtual environment

```
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
```

Some of the Transformer outputs generated based on previous conversation and print as new samples, so the number of samples would be larger than others.
For example:
```
--------------------example 53--------------------
Patient: is it safe to get care for my other medical conditions during this time ?
Reference: yes , it is important to continue taking care of your health and wellness . continue your medications , and do not change your treatment plan without talking to your healthcare provider . continue to manage your disease the way your healthcare provider has told you .
Predict: hello , your question on healthcare magic . in the of get cause as yes pneumonia .
--------------------example 54--------------------
Patient: is it safe to get care for my other medical conditions during this time ? [SEP] yes , it is important to continue taking care of your health and wellness . continue your medications , and do not change your treatment plan without talking to your healthcare provider . continue to manage your disease the way your healthcare provider has told you . [SEP] thanks a lot doctor .
Reference: no problem , let us know if you come across anything else .
Predict: brief opinion : ? covid - 19 in have from you like to - 19 . yes should if your . your in you like to covid - do with me ?
```

### Run evaluate script

```
python3 evaluate.py --o output/transformer_output.txt 
python3 evaluate.py --o output/gpt2_output.txt 
python3 evaluate.py --o output/Bart_output.txt 

```
