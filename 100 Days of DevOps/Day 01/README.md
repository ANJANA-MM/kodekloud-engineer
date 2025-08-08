# Day 01 - Create a User with a Non-Interactive Shell

✅ **Task:**  
Create a user with a non-interactive shell on a remote Linux server.

---

## 🛠️ Steps Followed:

1. **Login to the remote server via SSH:**

```bash
ssh username@remote_server_ip
```

2. **Create a user with a non-interactive shell:**

```bash
sudo useradd -s /sbin/nologin username
```
* -s option stands for:
    --shell → It specifies the login shell for the new user.

## 📚 Key Concepts:

🔍 What is a "login shell"?
A login shell is the program that runs when a user logs into the system, usually something like:

* /bin/bash (for interactive users)

* /bin/sh, /bin/zsh, etc.

🛡️ Why use /sbin/nologin?

Setting the shell to /sbin/nologin:

* Prevents the user from logging in interactively 

* They can’t run commands via SSH or terminal

* Commonly used for service accounts (e.g: a user that runs background tasks but doesn’t need login access)


## 🔗 Related Tags
#100DaysOfDevOps #Linux #KodeKloudEngineer #DevOpsJourney #ContinuousLearning
