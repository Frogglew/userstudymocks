# ARTICLE NO X: EXAMPLE

## Outcomes (if you do this, you'll get x, y, z)

## Prerequisites

## Step 1: Open Notebook on Studio

## Step 2: Connect to your workspace

```python
# Handle to the workspace
from azure.ai.ml import MLClient

# Authentication package
from azure.identity import DefaultAzureCredential

credential = DefaultAzureCredential()

# Get a handle to the workspace. You can find the info on the workspace tab on ml.azure.com
ml_client = MLClient(
    credential=credential,
    subscription_id="",  # this will look like xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
    resource_group_name="",
    workspace_name="",
)
```
## Step 3:

## (Optional) Connect to your Git respository

## Step n: Select or create an environment
In order to train, you'll need an environment. An environemtn is [TBD]. Azure Machine Learning offers different options that meet your needs.

- You can automatically generate an environment for several popular models (classification, blah, blah, etc)
- You can select from pre-configured environments available on Azure ML platform.
- You can create a custom environment.

For this tutorial, we will go with the first option. 

[More explanation needed]

## Step n+1: Use or create a training script

You have several ways to go about it

- You can automatically generate the initial training script for several popular models (classification, blah, blah, etc)
- You can write a custom notebook
- You can bring your exiting code/notebook

For this tutorial, we will assume you don't have a script yet for this [X] model. We are going to walk you through how to generate a default training script using AutoML. Why using AutoML?

Benefits
- efficiency
- blah
- blah

Once you generate the initial training script via AutoML, in the next article, you'll learn how to customize it to refine your model further. 

<AUTO ML CODE GOES HERE>
  
## Step n+2: Create a control script to submit the training job

## Step n+3: Pick the best model out of the initial training
