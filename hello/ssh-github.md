# `ssh-github.md`

## ❄ Instructions

1) Create a GitHub account and log in
    - You can use an existing GitHub account if you want
3) Set up a commit email on GitHub following these [instructions](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address#setting-your-commit-email-address-on-github).
    - If you choose to make your email private in step (5) above, then your commit email will be the `...@users.noreply.github.com`
4) Save your commit email in a `.txt` file for later
---
5) Generate a SSH key and add it to your ssh-agent following these [instructions](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
    - Windows users should follow the linux instructions in their WSL terminal
    - Everyone can skip the "Generating a new SSH key for a hardware security key" section
6) Add the SSH keys to your GitHub account following these [instructions](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
    - Windows users should follow the linux instructions in their WSL terminal
7) Take a screenshot after you finish adding the keys
8) Edit the screenshot to censor the key entries
---
9) Open your terminal
10) Run `git config --global user.name "Your Name"` where "Your Name" is your GitHub username
11) Run `git config --global user.email commit@email.com` where "commit@email.com" is your commit email from step (2) of these instructions.
    - Do not put quotes around your email in the above command!
12) Run `git config --global core.sshCommand "ssh -i path-to-your-private-key"` where `path-to-your-private-key` might look something like `~/.ssh/id_ed25519` if you accepted the default file name in step (5).
13) Run `git config --edit --global` to view your global `.gitconfig` file in vim in your terminal
14) Take a screenshot showing the username and email you added
    - If you are a Windows user using WSL, then you need to click outside the terminal to take a screenshot
15) Exit vim by entering `:q`

## 🌸 FAQ

### What if I see an error message like this when trying to clone a repo after following all these steps?

> The authenticity of host 'github.com (140.82.112.4)' can't be established.  
> ECDSA key fingerprint is SHA256:p2QAMXNIC1TJYWeIOttrVc98/R1BUFWu3/LiyKgUfQM.  
> Are you sure you want to continue connecting (yes/no)?  

---

Double-check if the key fingerprint matches GitHub's key fingerprints [here](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/githubs-ssh-key-fingerprints). If so, then type "yes" and git should finishing cloning the repo for you with some message like this:

> Warning: Permanently added 'github.com,140.82.112.4' (ECDSA) to the list of known hosts.

Your repo should still be cloned successfully though.

### Why does git ask me for my username after I initialize a new repository?

Because we are using ssh as our credentials, you should also try to use "ssh syntax" whenever possible. For example, you should run

```
git remote add origin git@github.com:your-username/your-repo-name
```

instead of

```
git remote add origin https://github.com/your-username/your-repo-name
```

Also don't forgot to do step (9) in the instructions so that git knows where to find your private ssh key!

## 🌸 Submission

- screenshot of your [SSH and GPG keys page](https://github.com/settings/keys) **with your entries blurred or covered** (for example, you can draw a rectangle over the key entries using ms paint or similar software on your machine)
- screenshot of your global `.gitconfig` file **with your email blurred or covered** (for example, you can draw a rectangle over email using ms paint or similar software on your machine)

## ❄ References

- [Connecting to GitHub with SSH | GitHub docs](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
- [How to have 2 or more GitHub accounts on one machine (Windows) | Linh Nguyen My | Medium](https://medium.com/@pinglinh/how-to-have-2-github-accounts-on-one-machine-windows-69b5b4c5b14e)
    - View in private browsing if Medium is blocking you
