# `ssh-github.md`

## ❄ Instructions

1) Log into GitHub
2) Set up a commit email on GitHub following these [instructions](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address#setting-your-commit-email-address-on-github).
    - If you choose to make your email private in step (5) above, then your commit email will be the `...@users.noreply.github.com`
3) Save your commit email in a `.txt` file for later
---
4) Generate a SSH key and add it to your ssh-agent following these [instructions](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
    - Windows users should follow the linux instructions in their WSL terminal
    - Everyone can skip the "Generating a new SSH key for a hardware security key" section
---
5) Add the SSH keys to your GitHub account following these [instructions](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
    - Windows users should follow the linux instructions in their WSL terminal
6) Take a screenshot after you finish adding the keys
7) Edit the screenshot to censor the key entries
---
6) Open your terminal
7) Run `git config --global user.name "Your Name"` where "Your Name" is your GitHub username
8) Run `git config --global user.email commit@email.com` where "commit@email.com" is your commit email from step (2) of these instructions.
    - Do not put quotes around your email in the above command!
9) Run `git config --edit --global` to view your global `.gitconfig` file in vim in your terminal
10) Take a screenshot showing the username and email you added
    - If you are a Windows user using WSL, then you need to click outside the terminal to take a screenshot
11) Exit vim by entering `:q`

## 🌸 Submission

- screenshot of your [SSH and GPG keys page](https://github.com/settings/keys) **with your keys blurred or covered** (for example, you can draw a rectangle over the key entries using ms paint or similar software on your machine)
- screenshot of your global `.gitconfig` file **with your email blurred or covered** (for example, you can draw a rectangle over the key entries using ms paint or similar software on your machine)

## ❄ References

- [Connecting to GitHub with SSH | GitHub docs](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
