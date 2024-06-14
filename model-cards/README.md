# Model Cards

Model cards are summary documents for machine learning models that improve transparency for those who are considered technical and those who are not.  Stakeholders, developers, product owners, policy makers can all use a model card to get a better understanding of the model, to make it seem less like a black box.  

These are the suggested six sections:
1. Model details
1. Intended use
1. Performance metrics
1. Training data
1. Quantitative analysis
1. Ethical considerations and recommendations

But the format varies widely from team to team.  

## Model Card Examples 
1. [Gradient Boost Classifier Model](/model-cards/examples/model-card-breast-cancer-wisconsin-diagnostic.pdf) (using the Breast Cancer Wisconsin Diagnostic dataset) 
1. [Claude 2](https://www-cdn.anthropic.com/files/4zrzovbb/website/bd2a28d2535bfb0494cc8e2a3bf135d2e7523226.pdf)
1. [GPT-3](https://github.com/openai/gpt-3/blob/master/model-card.md?ref=nocode.ai)

## Model Card How To

### Model Card Toolkit
The [Model Card Toolkit](https://github.com/tensorflow/model-card-toolkit) is a Python library that can be installed where needed to generate an HTML version of a model card. A [sample notebook](https://github.com/tensorflow/model-card-toolkit/blob/main/model_card_toolkit/documentation/examples/Scikit_Learn_Model_Card_Toolkit_Demo.ipynb) demonstrates how to create a model card from a Gradient Boost Classifier model. The notebook was last changed in 2023 and needed a few updates to be runnable in 2024 (using Google Colab and Python 3).  The installs in the first cell should be changed to match the code block below.  

The flag `--use-deprecated=legacy-resolver` was needed for the model-card-toolkit. 

```
!pip install --upgrade pip
!pip install model-card-toolkit --use-deprecated=legacy-resolver
!pip install --upgrade seaborn 'scikit-learn>=0.22.0'
```
