# Sentiment-Analyzer-Gadio-HuggingFace

### STEPS:
## How to run? 
### STEP 01- Create a conda environment after opening the repository
```bash
conda create -p sentimentanalyzerenv python -y
```

```bash
source activate ./sentimentanalyzerenv
```

### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```

### STEP 03- run application
```bash
Python app.py
```

##### after download move the model to code folder
```bash
cd /Users/mayankchugh/.cache/huggingface/hub/
```
###### copy your downloaded model name and path and paste it below (it already pasted for my workspace)
```bash 
sudo mv /Users/mayankchugh/.cache/huggingface/hub/models--distilbert--distilbert-base-uncased-finetuned-sst-2-english /Users/mayankchugh/gitRepos/mayankchugh.learning/Sentiment-Analyzer-Gadio-HuggingFace/Models/models--distilbert--distilbert-base-uncased-finetuned-sst-2-english
```

### Prompt to create content for excel
```bash
I need an excel contains one column as "Review". this column should contain atleast 10 customer comments of product. 5 comments should be positive and 5 negative. comments should not be more that 1 liner.
```

### Prompt to create code
```bash
Write a Python code that reads the Excel file based on the Excel file path provided as input for the function. the file has reviews; it should call a function get sentiment and return me the data frame that contains both reviews as well as corresponding sentiment. Also, Check if the 'Review' column is in the Dataframe - raise an error if it does not exist. add gradio as frontend for user to upload file
```

### Prompt to add plot chart to be added

```bash
Add a Python function which takes a dataframe as an input and contains 2 columns, (Review & Sentiment - Positive, Negative) and it will return an object of bar chart that can be passed to the Gradio tool to plot a chart in gradio UI
```


[Gradio documentation link](https://www.gradio.app/docs/gradio/file)