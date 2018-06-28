# Installing Toolbox using vagrant

1. Install requirements
- [Virtual box](http://www.virtualbox.org) (Version 5.1 +)
- [Vagrant](http://www.vagrantup.com) (Version 1.9.2 or +)


2. Clone repository and start provision
```
git clone https://github.com/marvin-ai/marvin-vagrant-dev.git
cd marvin-vagrant-dev
```

3. Prepare dev (engine creation) box
```
vagrant up dev
vagrant ssh dev
```
Wait for provision process and follow interactive configuration script after access the dev box using vagrant ssh command.

4. The marvin source projects will be on your home folder, to compile and use the marvin toolbox
```
workon python-toolbox-env
make marvin
```