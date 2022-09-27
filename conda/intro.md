# `intro.md`

Here's a quickstart to using conda virtual environments for the [TTS](https://www.techtalentsouth.com/) data science program.

---

## Clone this repo

Open a terminal. Navigate to where you want to clone this repo. Then run

```
git clone https://github.com/Ai-Yukino/tts-ds-ai
```

## Install the conda `tts` virtual environment

Navigate to the `conda` folder. For example, you might run

```
cd tts-ds-ai/conda
```

Next run

```
conda env create -f tts.yml
```

to install the `tts` environment. It could take a minute or so.

## Activate the `tts` environment

Run

```
conda activate tts
```

**Note**: After you've done the previous step, you don't need to navigate to the `tts-ds-ai/conda` folder to activate this `tts` environment. You can activate this environment from any folder in your terminal.

## Open a Jupyter notebook

Navigate to the folder with the jupyter notebook files you want to open. For example, maybe `tts-ds-fundamentals-course`. Then run

```
jupyter lab --no-browser
```

and click on one of the links that shows up in your terminal to view the notebook.

## References

- [Command reference | conda docs](https://docs.conda.io/projects/conda/en/latest/commands.html)
- [Install Jupyter | Jupyter docs](https://jupyter.org/install)
