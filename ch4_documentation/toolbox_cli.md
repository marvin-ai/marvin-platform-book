# Toolbox CLI

### Command line interface
Usage: marvin [OPTIONS] COMMAND [ARGS]

Options:
```
  --debug       #Enable debug mode.
  --version     #Show the version and exit.
  --help        #Show this command line interface and exit.
```

Commands:
```
  engine-generate     #Generate a new marvin engine project.
  engine-generateenv  #Generate a new marvin engine environment.
  engine-grpcserver   #Marvin gRPC engine action server starts.
  engine-httpserver   #Marvin http api server starts.
  hive-dataimport     #Import data samples from a hive databse to the hive running in this toolbox.
  hive-generateconf   #Generate default configuration file.
  hive-resetremote    #Drop all remote tables from informed engine on host.
  notebook            #Start the Jupyter notebook server.
  pkg-bumpversion     #Bump the package version.
  pkg-createtag       #Create git tag using the package version.
  pkg-showchanges     #Show the package changelog.
  pkg-showinfo        #Show information about the package.
  pkg-showversion     #Show the package version.
  pkg-updatedeps      #Update requirements.txt.
  test                #Run tests.
  test-checkpep8      #Check python code style.
  test-tdd            #Watch for changes to run tests automatically.
  test-tox            #Run tests using a new virtualenv.
```