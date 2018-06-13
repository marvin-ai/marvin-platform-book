# Working in an existing engine

1. If you don't have an engine locally, clone one to your local machine

2. On Python Toolbox environment, set VirtualEnv and get to engine's path
```
marvin engine-generateenv /path/to/engine/
workon <engine_name>-env
```
3. Test your engine
```
marvin test
```
4. Bring up the notebook and access it from your browser
```
marvin notebook
```