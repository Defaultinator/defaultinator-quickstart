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

## Build

```
$ docker-compose build
```

## Run

### Base configuration
```
$ docker-compose up
```

### Development configuration

This is the base configuration with the addition of the storybook component.
```
$ docker-compose -f docker-compose.yml -f docker-compose.dev.yml up
```
