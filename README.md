# Google Doc AI Demo


## Getting started


## Pre-requisites
python 3.9

pip install streamlit
pip install streamlit-aggrid

Setup Google Cloud Vision using the instructions at https://cloud.google.com/vision/docs/ocr

Setup Google Document AI using the instructions at https://cloud.google.com/document-ai

## Steps to folow

1. To read the PDF file and create .csv files
```
export GOOGLE_APPLICATION_CREDENTIALS="path to security credentials json file"
python doc_ai_table.py --pdf <path to pdf file> --folder <output folder>
```
Check the csv files produced for each table detected in the PDF.
Also check the header.json produced based on form-fields (key value pairs) detected in first page of PDF

2. Run the UI demo 
```
streamlit run app.py
```
