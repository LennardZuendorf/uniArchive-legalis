# README for the coursework
This project contains many files and notebooks, so here is a short overview of the most important ones and how to use them.

## Note about Huggingface
I heavily relied on huggingface in my work, which is reflected throughout my notebooks. The hub can be used without login if data only gets pulled from there. See more about Dataset in the official [docs](https://huggingface.co/docs/datasets/index). The same goes for the BERT model, login is only needed to upload it to the hub.

## Structure
The project is structured into three main folders: `Data`, `Model` and `App`/`Legalis`. Each contains the notebook/python files for the respective part of the project.

### Data
The data folder contains the notebooks for cleaning and enhancing the data with the CHatGPT API. The data is then saved in the `data` folder in the root directory, which I only did for reproductive, in production I exclusively used the huggingface hub. 

#### Notebooks:
- `Legalis_Dataset` contains the code for initial cleaning of the data from openlegaldata.io
- `Legalis_Extractor` contains the code for extracting labels from the cleaned data with the CHatGPT API

#### Files
- `legalis_dataset.csv` contains the final, enhanced data used for training the models
- `openlegaldata-bulk-data.csv` (not included in moodle upload because it's 7 GB) contains the raw data from openlegaldata.io, see [Huggingface](https://huggingface.co/datasets/LennardZuendorf/openlegaldata-bulk-data) for reference
- `three-split-dataset.csv` contains the part of the dataset where I was able to split the content into three parts (tenor, facts, reasoning)
- `two-split-dataset.csv` contains the part of the dataset where I was able to split the content into two parts (tenor, reasoning)

### Model
The model folder contains the notebooks for training the models. The BERT model is also uploaded to the huggingface hub, see [here](https://huggingface.co/LennardZuendorf/legalis-BERT) for reference.

#### Notebooks:
- `Legalis_BERT_Predictor` contains the code for fine-tuning a German BERT model and uploading it to the huggingface hub
- `Legalis_scitkit_Predictor` contains the code for training a Naive Bayes Multimodal Model and fine-tuning, training a Random Forest Model

### Legalis
The Legalis folder contains the code for the gradio app. The app is also uploaded to the huggingface hub, see [here](https://huggingface.co/spaces/LennardZuendorf/legalis) for reference. The code is extremely simple and mostly for showcase purposes. With much work you can also use a scikit-learn model for it, but the library has many faults and bugs, so I was not able to finish that part.