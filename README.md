# defaultinator-quickstart

## Setup

```
$ git clone --recurse-submodules git@github.com:Defaultinator/defaultinator-quickstart.git
$ cd defaultinator-quickstart
```

If you cloned the project and forgot `--recurse-submodules`, you may run the following command to initialize, fetch and checkout any nested submodules.
```
git submodule update --init --recursive
```

### Base configuration
#### Build and start containers

```
$ docker-compose up --build
```

#### Stop containers
```
$ docker-compose down
```

### Development configuration
#### Build and start containers

This is the base configuration with the addition of the storybook component. Before running ensure you enter each submodule directory and follow the instructions for installing dependencies.
```
$ docker-compose -f docker-compose.yml -f docker-compose.dev.yml up --build
```

#### Stop containers
```
$ docker-compose -f docker-compose.yml -f docker-compose.dev.yml down
```
