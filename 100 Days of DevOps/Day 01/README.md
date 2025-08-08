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
This ensures the user exists on the system but cannot log in interactively - often used for service accounts or automation tasks where login is not required.

## 📚 Key Concepts:
* /sbin/nologin: A shell that immediately exits and prevents interactive login.

* Used to improve security by restricting shell access.

## 🔗 Related Tags
#100DaysOfDevOps #Linux #KodeKloudEngineer #DevOpsJourney #ContinuousLearning
