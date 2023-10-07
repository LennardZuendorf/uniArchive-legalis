# legalis
#### This is the mono repo for the legalis project. The focus of the project is prediction work and data science around German Court cases. Currently, this repo contains a folder for Data, Model, and App. Each contains the notebook/python files for the respective part of the project.

#### The project contains two notebooks for cleaning and enhancing with the CHatGPT API, as well as one notebook used for training a random forest and Naive Bayes Multimodal Model and one for a BERT Classification Model fine-tuned on top of a German BERT. The latter is also running in hugging face spaces.

> ℹ️
> This is an archive of tasks done as part of my studies.

##### Ultimately I was able to predict the outcome of 60% of the court cases. But to be fair, the methods are not completely scientifically corrent.

## 🔗 Links:

**[Interactive Model Demos on Huggingface](https://huggingface.co/spaces/LennardZuendorf/legalis)**

**[BERT Model on Huggingface](https://huggingface.co/LennardZuendorf/legalis-BERT)**

**[Random Forest Classifier on Huggingface](https://huggingface.co/LennardZuendorf/legalis-scikit)**

**[Labeled Dataset on Huggingface](https://huggingface.co/datasets/LennardZuendorf/legalis)**

## 🏗️ Tech Stack:

**Language/Platform:** Python, JupyterNotebook

**Noteable Libaries:** 🤗Datasets, 🤗Evaluate, scikit-learn, 🤗Transformers

**Base Dataset:** [OpenLegalData](https://huggingface.co/datasets/LennardZuendorf/openlegaldata-bulk-data)

## 👨‍💻 Author and Credits:

**Author:** [@LennardZuendorf](https://github.com/LennardZuendorf)

- This project is part of a course in HTW Berlin's Business Computing Bachelor Program ("Unternehmenssoftware")
