# Creating a new engine
1. To create a new engine
```
workon python-toolbox-env
marvin engine-generate
```
Respond the interactive prompt and wait for the engine environment preparation, and don't forget to start dev box before if you are using vagrant.

2. Test the new engine
```
workon <new_engine_name>-env
marvin test
```
3. For more informations
```
marvin --help
```
4. Youtube Tutorial

[![Creating first engine](http://img.youtube.com/vi/p7yiLh2uLlQ/0.jpg)](https://www.youtube.com/watch?v=p7yiLh2uLlQ "Creating first engine")
