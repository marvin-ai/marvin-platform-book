# General Overview

Here are the components

# DAFSE

The DASFE design pattern stands for Data Acquisition, Selection, Feedback and Evaluation.
In Marvin, the DASFE pattern is represented by the image below. Each box, which we call an Action, holds code written by the user.

![](https://raw.githubusercontent.com/marvin-ai/marvin-paper/master/from-exploratory-models-to-productions/fig/marvin-dase.png)

# Engine Executor

The [engine executor](https://github.com/marvin-ai/marvin-engine-executor) is the component responsible for coordinating execution of the steps (Actions) in a Marvin engine. The engine-executor is able to communicate with engines through the gRPC protocol.

# Artefacts

Datasets and model(s) are shared between Engine Actions, which are persisted and versioned.

# Marvin Notebook Extension

In order to facilitate development of the engine, Jupyter Notebook is integrated into Toolbox. The Marvin notebook extension allows the user to write their code in Notebooks and push updates directly to the Actions.