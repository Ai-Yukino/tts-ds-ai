# `WSL.md`

## ❄ Overview

We're going to

- install WSL with the "Ubuntu" distribtion,
- find the `.bashrc` file, and
- take a screenshot of the contents of the `.bashrc` file.

## 🌸 Instructions

1) Install Windows Terminal following these [instructions](https://github.com/Ai-Yukino/tts-ds-ai/blob/main/hello/windows-terminal.md).
2) Open Windows Terminal in administrative mode.
3) Run `dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart` to enable WSL on Windows.
4) Run `dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart` to enable the Virtual Machine feature for Windows.
5) Install this [Windows update](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi).
6) Run the command `wsl --install -d ubuntu`.
7) After Ubuntu is installed in a new window that pops up, create a username and password for the Ubuntu virtual OS. (**Note**: Your username cannot start with a capital letter)
8) Close that above window.
9) Close Windows Terminal.
10) Open Windows Terminal again (doesn't need to be in administrative mode).
11) Open a WSL/Ubuntu tab.
12) Make sure you are in the home directory, i.e. the "~" directory. If not, run `cd ~`.
13) Run `explorer.exe .` and don't forget the period at the end!
14) Open `.bashrc` in your prefered Windows text editor.
15) Take a screenshot of the `.bashrc` file in your text editor.

## ❄ Submission

A screenshot of your `.bashrc` file opened with a Windows text editor

## 🌸 References

- [Install Linux on Windows with WSL | Microsoft docs](https://docs.microsoft.com/en-us/windows/wsl/install)
- [Manual installation steps for older versions of WSL](https://docs.microsoft.com/en-us/windows/wsl/install-manual)

## ❄ Sample solution video

TBA
