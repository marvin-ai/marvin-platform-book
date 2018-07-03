# Installing Toolbox as Ubuntu user

1. Libsasl2-dev, Python-pip and Graphviz installation
```
sudo apt-get install libsasl2-dev python-pip graphviz -y
```
2. VirtualEnvWrapper Installation
```
sudo pip install --upgrade pip
sudo pip install virtualenvwrapper --ignore-installed six
```
3. Spark installation
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
4. Set environment variables
```
echo "export WORKON_HOME=$HOME/.virtualenvs" >> $HOME/.bash_profile
echo "export MARVIN_HOME=$HOME/marvin" >> $HOME/.bash_profile
echo "export MARVIN_DATA_PATH=$HOME/marvin/data" >> $HOME/.bash_profile
echo "source virtualenvwrapper.sh" >> $HOME/.bash_profile

source ~/.bash_profile
```
5. Clone and install python-toolbox

```
mkdir $MARVIN_HOME
mkdir $MARVIN_DATA_PATH
cd $MARVIN_HOME

git clone https://github.com/marvin-ai/marvin-python-toolbox.git
cd marvin-python-toolbox

mkvirtualenv python-toolbox-env
setvirtualenvproject

make marvin
```

6. Test the installation
```
marvin test
```

7. Youtube tutorial

[![Python Toolbox Install](http://img.youtube.com/vi/2iljFG9EZ_Q/0.jpg)](https://www.youtube.com/watch?v=2iljFG9EZ_Q "Python Toolbox Install")