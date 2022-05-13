# Miniconda

## Anaconda vs. Miniconda

Miniconda comes with Python and conda for managing packages and environments. This is the bare minimum.

Anaconda starts with Miniconda, but additionally it installs a bunch of packages suited for data science such as pandas and numpy. Anaconda could be very easy and user-friendly, and you can jumpstart, but because it comes with a suite of pre-installed packages, it is very heavy, and many times you don't actually end up using all those packages. Also, when you need to deploy your work and figure out absolutely necessary minimal dependency list, starting from the bare minimum and installing packages as you needed is a better approach in my opinion.

## Installation

From a terminal window, enter the following command to download Miniconda:

```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

Install Miniconda:

```bash
chmod +x Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```

Once you have installed Miniconda, open a new terminal window. Your prompt should begin with a text `(base)`.

For example:

```
(base) -bash-4.2$
```

Make sure you have a working conda by running the following command:

```bash
conda --version
```
