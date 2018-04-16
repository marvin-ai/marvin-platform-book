# DASFE

The DASFE design pattern stands for Data Acquisition, Selection, Feedback and Evaluation.
In Marvin, the DASFE pattern is represented by the image below. Each box, which we call an Action, holds code written by the user.

![](https://raw.githubusercontent.com/marvin-ai/marvin-paper/master/from-exploratory-models-to-productions/fig/marvin-dase.png)

# Toolbox

The toolbox helps the user develop, test, and run their built engine.
There are separate toolboxes for each language. For example, the Python Toolbox.

# Engine

The Engine is the Marvin application, the result of user's implementation, including code, datasets(artifacts), models, etc.

# Engine Executor

The engine executor is the component responsible for coordinating execution of the steps (Actions) in a Marvin engine. The engine-executor is able to communicate with engines through the gRPC protocol.

# Artifacts

Datasets are shared between Engine Actions, which are persisted and versioned.

# Notebook extension

In order to facilitate development of the engine, Jupyter Notebook is integrated into Toolbox. The Marvin notebook extension allows the user to write their code in Notebooks and push updates to directly to the Actions.
