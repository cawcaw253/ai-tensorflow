# Info

## Install (mac)

### install Python

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

### install Miniforge

* Install from Miniforge homepage: https://github.com/conda-forge/miniforge

```
bash Miniforge3-MacOSX-arm64.sh
```

### create Conda environment

```
conda env create --file=environment.env --name=workspace
```

### activate environment

```
conda activate TensorFlowWorkspace
```

### install TensorFlow and TensorFlow Addons for macOS

```
pip install --upgrade --force --no-dependencies https://github.com/apple/tensorflow_macos/releases/download/v0.1alpha3/tensorflow_macos-0.1a3-cp38-cp38-macosx_11_0_arm64.whl https://github.com/apple/tensorflow_macos/releases/download/v0.1alpha3/tensorflow_addons_macos-0.1a3-cp38-cp38-macosx_11_0_arm64.whl
```

### install Jupyter Notebooks

```
conda install notebook -y
```

## Running

### activate conda environment

```
conda activate TensorFlowWorkspace
```

### running Jupyter

```
jupyter notebook
```

## Shut Down

### shut down Jupyter Notebook

```
Ctrl + C
```

### deactivate conda environment

```
conda deactivate
```

## Refer to

* https://alexmanrique.com/blog/development/2021/03/05/installing-jupyter-in-macbook-air-m1.html
* https://medium.com/gft-engineering/macbook-m1-tensorflow-on-jupyter-notebooks-6171e1f48060