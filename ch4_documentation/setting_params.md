# Setting Environmental Variables

To set up environmental parameters or variables on Marvin it's recommended 
to use the argument ```params``` that is present on every engine actions.

## Setting up params
You may edit the file *engine.params* that is located at the root directory 
of your engine. You must insert params as a dictionary:

```
{
    "login" : "marvin",
    "password": "123455"
}
```

## Loading params
Params are loaded as an argument on your engine execution. Then, inside your 
code you must do ```params.get("login")``` or ```params["login"]``` to access 
those variables.

## Samples
* [Example of *engine.params* file](https://github.com/marvin-ai/marvin-public-engines/blob/master/iris-species-engine/engine.params)
* [Example of loading params on **Acquisitor and Cleaner**](https://github.com/marvin-ai/marvin-public-engines/blob/master/iris-species-engine/marvin_iris_species_engine/data_handler/acquisitor_and_cleaner.py)

**Notice that  if you are running your actions using an API, you may alse set params at 
the the API body. These params will overwrite the <i>engine.params</i> file.**

