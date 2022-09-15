# `conda.md`

## ❄ Instructions

We will

- Install Miniconda
- Create a conda virtual environment with the latest version of python
- Export a `.yml` config file of that environment

1) Install Miniconda:
    - [macOS instructions](https://conda.io/projects/conda/en/latest/user-guide/install/macos.html)
    - [Linux instructions](https://conda.io/projects/conda/en/latest/user-guide/install/linux.html)
    - Windows:
      - Install Windows Terminal following these [instructions](https://github.com/Ai-Yukino/tts-ds-ai/blob/main/hello/windows-terminal.md)
      - Install WSL with the "Ubuntu" distribution following these [instructions](https://github.com/Ai-Yukino/tts-ds-ai/blob/main/hello/WSL.md)
      - Follow the linux instructions and install Miniconda on your Ubuntu virtual OS
        - Make sure to download the latest Linux Miniconda installer [here](https://docs.conda.io/en/latest/miniconda.html#latest-miniconda-installer-links)
        - You can download the installation files by running `wget "path-to-file"` or `curl "path-to-file"`
3) Create a conda virtual environment with the latest version of python
4) Export a `.yml` config file of that environment

## 🌸 Submission

A `.yml` config file of your conda environment with the latest version of python

## ❄ Tips

- Run `conda create --name tts-ds` to create an empty conda virtual environment named "tts-ds". You can replace "tts-ds" with whatever name you prefer.
- Run `conda activate base` to activate the `base` environment. You can replace `base` to be the name of whatever environment you want to activate as long as you have created it in your local machine.
- Run `conda search python` to see all the available versions of python you can install
- Run `conda install python=3.10.2` to install python version "3.10.2".
- Run `conda env export --from-history > env.yml` to export a config file named `env.yml`.

## 🌸 References

### conda docs

- [Concepts](https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/index.html)
- [Cheat sheet](https://docs.conda.io/projects/conda/en/latest/user-guide/cheatsheet.html)
- [Command reference](https://docs.conda.io/projects/conda/en/latest/commands.html)

### Other

- [The Good Research Code Handbook | goodresearch.dev](https://goodresearch.dev/index.html)

## ❄ Sample solution video

TBA
