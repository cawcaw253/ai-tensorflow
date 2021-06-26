# Info

## Install (mac)

### Installing Python

```
brew install pyenv 
```

```
pyenv install 3.9.1
```

with the following command, we can add the initialization of pyenv new values into the .zshrc file, this way we don’t have to type the same command everytime we open a new terminal, in my case I use iterm2.

```
echo 'eval "$(pyenv init -)"' >> .zshrc
```

```
pyenv global 3.9.1
```

### Installing Jupyter

```
pip3 install jupyter
```

## Running Jupyter

```
jupyter notebook
```
