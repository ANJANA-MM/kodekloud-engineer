# Day 02 - Create a Temporary User Account

✅ **Task:**  
Create a temporary user account with an expiry date on a remote Linux server.

---

## 🛠️ Steps Followed

1. **Login to the remote server via SSH:**

```bash
ssh username@remote_server_ip
```
2. **Create a temporary user account with an expiry date:**

```bash
sudo useradd -e YYYY-MM-DD username
```

🔹 Example:
```bash
sudo useradd -e 2025-09-18 sam
```
* -e stands for expiry date
* allowing you to set when the user account will be automatically disabled.

3. **Verify the account expiry:**

```bash
sudo chage -l sam
```

Output:

```bash
Account expires : Sep 18, 2025
```
* This confirms the expiry date has been successfully applied.

## 📚 Key Concepts
* Temporary accounts are useful for:
      - contractors
      - interns
       - or time-bound tasks.

* The account gets automatically disabled after the expiry date, improving security.

* 'chage' helps you review and manage account aging and expiration policies.

## 🔗 Related Tags
#100DaysOfDevOps #Linux #UserManagement #KodeKloudEngineer #ContinuousLearning
