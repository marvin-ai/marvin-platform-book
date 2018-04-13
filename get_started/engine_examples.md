# Running a example engine 
1. Clone example engine from repository
```
git clone https://github.com/marvin-ai/engines.git
```
2. Generate a new marvin engine environment for Iris species engine
```
workon python-toolbox-env
marvin engine-generateenv ../engines/iris-species-engine/
```
3. Run the Iris species engine
```
workon iris-species-engine-env
marvin engine-dryrun 
```

For more examples: https://github.com/marvin-ai/marvin-public-engines