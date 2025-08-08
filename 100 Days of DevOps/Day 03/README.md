# 🚀 Day 03 - 100 Days of DevOps with KodeKloud

## 🔐 Task
**Disable direct SSH root login to a Linux server**

---

## 🛠️ Steps Followed

1. **Login to the remote server via SSH**  
   (not as the root user, but with a user that has sudo privileges):
   ```bash
   ssh user@server_ip
   ```

2. **Edit the SSH configuration file** 
   * Open the file using vi editor:
    ```bash
    sudo vi /etc/ssh/sshd_config
    ```
   
   * Enter insert mode: 
     Press i

  * Locate the line:
    ```bash
    PermitRootLogin yes
    ```

  * Update that line to:
    ```bash
    PermitRootLogin no
    ```

  * Save & Exit
      - Press Esc (To enter the command mode)
      - Type :wq! and hit Enter (To save & exit)


3. **Restart the SSH service** 
     ```bash
     sudo systemctl restart sshd
     ```

## 🎯 Why This Matters
Disabling root login:

* Prevents unauthorized access

* Enforces least privilege access

## 🔗 Related Tags
#100DaysOfDevOps #Linux #KodeKloudEngineer #ContinuousLearning
