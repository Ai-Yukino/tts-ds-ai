# `ssh-github.md`

## ❄ Instructions

1) Create a GitHub account and log in
    - You can use an existing GitHub account if you want
3) Set up a commit email on GitHub following these [instructions](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address#setting-your-commit-email-address-on-github).
    - If you choose to make your email private in step (5) above, then your commit email will be the `...@users.noreply.github.com`
4) Save your commit email in a `.txt` file for later
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
9) Run `git config --global core.sshCommand = ssh -i path-to-your-private-ssh-key` where `path-to-your-private-ssh-key` might look something like `~/.ssh/id_25519` if you accepted the default name in step (4).
10) Run `git config --edit --global` to view your global `.gitconfig` file in vim in your terminal
11) Take a screenshot showing the username and email you added
    - If you are a Windows user using WSL, then you need to click outside the terminal to take a screenshot
12) Exit vim by entering `:q`

## 🌸 FAQ

**Question**: What if I see an error message like this when trying to clone a repo after following all these steps?

> The authenticity of host 'github.com (140.82.112.4)' can't be established.  
> ECDSA key fingerprint is SHA256:p2QAMXNIC1TJYWeIOttrVc98/R1BUFWu3/LiyKgUfQM.  
> Are you sure you want to continue connecting (yes/no)?  

**Answer**: Double-check if the key fingerprint matches GitHub's key fingerprints [here](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/githubs-ssh-key-fingerprints). If so, then type "yes" and git should finishing cloning the repo for you with some message like this:

> Warning: Permanently added 'github.com,140.82.112.4' (ECDSA) to the list of known hosts.

Your repo should still be cloned successfully though.

## 🌸 Submission

- screenshot of your [SSH and GPG keys page](https://github.com/settings/keys) **with your entries blurred or covered** (for example, you can draw a rectangle over the key entries using ms paint or similar software on your machine)
- screenshot of your global `.gitconfig` file **with your email blurred or covered** (for example, you can draw a rectangle over email using ms paint or similar software on your machine)

## ❄ References

- [Connecting to GitHub with SSH | GitHub docs](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
