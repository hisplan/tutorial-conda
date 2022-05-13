# Conda Environments

With conda, you can create multiple environments that have different versions of Python and/or packages installed in them.

## Create Environment

We will create a new environment calledd `prj-abc` and install Python 3.8, pip, and Jupyter Notebook:

```bash
conda create -n prj-abc python=3.8 pip jupyter
```

## List Environments

To see a list of all of your environments:

```bash
conda env list
```

## Activate/Deactivate Environment

Switching between environments is called activating the environment:

```bash
conda activate prj-abc
```

```bash
conda deactivate
```

## Remove Environment

```bash
conda env remove -n prj-abc
```

## Examples

For your deep learning projects, suppose you need to use PyTorch for `prj-abc` and TensorFlow for `prj-xyz`.

### prj-abc

```bash
conda create -n prj-abc python=3.10 pip jupyter
conda activate prj-abc
conda install pytorch torchvision torchaudio cudatoolkit=11.3 -c pytorch
```

### prj-xyz

```bash
conda create -n prj-xyz python=3.10 pip jupyter
conda activate prj-xyz
pip install tensorflow
```
