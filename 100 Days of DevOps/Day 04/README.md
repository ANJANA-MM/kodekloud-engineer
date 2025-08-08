# ✅ Day 04 - 100 Days of DevOps Journey with KodeKloud

## 🔐 Task:
Grant executable permissions to a script on a Linux server, and ensure that **all users** have the capability to execute it.

---

## 🛠️ Steps Followed:

1. **Login to the remote server via SSH**  
   ```bash
   ssh user@server_ip
   ```

2. **Give both read & execute permissions to all users to execute the script**
   ```bash
   sudo chmod a+rx script1.sh
   ```
 
## ❓ Why do we need to provide both read & execute permissions?

* r → Allows the shell to read the contents of the script file & interpret them

* x → Allows the OS to execute the file as a script

## 📎 Related tags

#100DaysOfDevOps #Linux #KodeKloudEngineer #ContinuousLearning
