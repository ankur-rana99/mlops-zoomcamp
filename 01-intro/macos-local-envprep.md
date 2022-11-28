# MacOS | Environment preparation

## Pre step : Install home brew 
run command :
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"


## Step 1: Download and install the Anaconda distribution of Python
```sh
brew install anaconda --cask
```

## Step 2: Set Environment Variables for conda

**Note:** if you have up to date terminal client 'zsh', make changes in `~/.zshrc` file, otherwise it gonna be named as `~/.bashrc`.

```sh
nano ~/.zshrc
```

And add following:

**Note:** `--cask` flag installs modules into `/usr/local` directory. If you installed anaconda into another directory, just change root path down below.

```sh
export PATH="/usr/local/anaconda3/bin:$PATH"
```

To execute changes:

```sh
source ~/.zshrc
```

## Step 3: Install Docker (docker-compose already included)

```sh
brew install docker --cask
```

## Step 4: Run Docker

```sh
docker run hello-world
```
