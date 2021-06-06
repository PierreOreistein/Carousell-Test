# Carousell Homework
## To Reproduce the Resulsts
In order to reproduce the results of the experiments, please install the dependancies with

```sh
pip install -r requirements.txt
```

> ⚠ WARNING:
> The data have not be uploaded on the Git repository. Please make sure you have access to the '.csv' containing the data before trying to reproduce the results.

[Optionnal] You can also install the pre-commit if you want to contribute.

```sh
pre-commit install
```

## Organisation of the Project

We divided our work in three notebooks:

    1 - **1-DATA-EXPLORATION** for the exploration of the data. In this notebook, we pay extra attention to the consistency of the data, the relationship between the different columns and we do an extensive analysis of the 'price' feature.
    
    2 - **2.1-TRANSFORMERS-MODEL-DEVELOPMENT-AND-TRAINING**, we implement a Tokenizer-Transformer model based on the pre-trained neural network model: 'Albertv2'. Unfortunately, despite a training on a GPU, our computationnal power was too limited for the training of such a model.
    
    3 - **2.2-TF-IDF-DEVELOPMENT-AND-TRAINING**. Being unsuccessfull with the Transformer, we implement in this notebook a more classic model based on TF-IDF combined with a balanced random forest. We achieved a decent score of on the validation set.
 
For enhance visualisation of the notebooks, we deployed a JupyterBook at 
 
 
## Roadmap

* Add MlFlow to do a tracking of our experimentations
* Test different type of Tokenizers (WordPiece) and check different combinaitions of their parameters.
* Use a better GOU for the training of the Transformer
* Further study the tokenization to use a tokenizer that corresponds to our vocabulary, maybe trained our own tokenizer?
* Use the correlation between some category_id (as they belong to the same l1_category_name) to tune the loss to take into account this correlation in a quadratic term
  
## Contact

* Name: Pierre Oreistein
* Email: pierre.oreistein@gmail.com
