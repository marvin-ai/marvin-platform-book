# DASFE

The DASFE design pattern, means Data Acquisition, Selection, Feedback and Evaluation.
In Marvin, the DASFE pattern is represented by the image below, each box is an Action where the user codes fit.

![](https://raw.githubusercontent.com/marvin-ai/marvin-paper/master/from-exploratory-models-to-productions/fig/marvin-dase.png)

# Toolbox

User toolbox, helps user to develop, test and run your built engine.
There is multiples toolboxs, one for each language, like the first one is Python Toolbox.

# Engine
Marvin application, result of user's implementation, including codes, datasets(artifacts), models and etc

# Engine Executor

This is the component responsible for coordinate execution of the steps (actions) in a Marvin engine. The engine-executor is able to communicate with engines through gRPC protocol.

# Artifacts

Datasets shared between Engine Actions, which are persisted and versioned.

# Notebook extension

In order to facilitate development of the engine, Jupyter Notebook is integrated into Toolbox.
