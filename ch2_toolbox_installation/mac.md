# Installing Toolbox as MacOS user

1. Toolbox will need some OS dependencies
```
sudo easy_install pip
brew install openssl graphviz
```

2. We strongly recommend the use of VirtualEnv and VirtualEnvWrapper
```
sudo pip install --upgrade pip
sudo pip install virtualenvwrapper --ignore-installed six
```

3. Spark installation (**Optional**)
```
curl https://d3kbcqa49mib13.cloudfront.net/spark-2.1.1-bin-hadoop2.6.tgz -o /tmp/spark-2.1.1-bin-hadoop2.6.tgz
sudo tar -xf /tmp/spark-2.1.1-bin-hadoop2.6.tgz -C /opt/
sudo ln -s /opt/spark-2.1.1-bin-hadoop2.6 /opt/spark
echo "export SPARK_HOME=/opt/spark" >> $HOME/.bash_profile
```

If you do not have /opt directory created, before unpacking spark, run:
```
sudo mkdir /opt
```

4. Marvin uses dafault values for these environment variables, but you can customize them (**Optional**)
```
echo "export WORKON_HOME=$HOME/.virtualenvs" >> $HOME/.bash_profile
echo "export MARVIN_HOME=$HOME/marvin" >> $HOME/.bash_profile
echo "export MARVIN_DATA_PATH=$HOME/marvin/data" >> $HOME/.bash_profile
echo "source virtualenvwrapper.sh" >> $HOME/.bash_profile
source ~/.bash_profile
```

5. Install python-toolbox
```
mkvirtualenv python-toolbox-env
setvirtualenvproject
pip install marvin-python-toolbox
```

6. Test the installation
```
marvin test
```

7. Youtube tutorial

[![Python Toolbox Install](http://img.youtube.com/vi/2iljFG9EZ_Q/0.jpg)](https://www.youtube.com/watch?v=2iljFG9EZ_Q "Python Toolbox Install")