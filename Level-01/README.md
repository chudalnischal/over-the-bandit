# OverTheWire: Bandit – Level 0 → Level 1

## 🧠 Objective

The goal of this level is to **connect to the Bandit server using SSH** and **find the password** for the next level (Level 1).

---

## 🔐 Login Information

- **Username:** `bandit0`
- **Hostname:** `bandit.labs.overthewire.org`
- **Port:** `2220`

---

## 🧪 Steps to Solve Level 0

### ✅ Step 1: Connect to the server

Use the following SSH command in your terminal:

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
#When prompted for a password, enter:

bandit0
```
💡 Tip: If you're using Windows, you can use PowerShell, Windows Terminal, or WSL (Windows Subsystem for Linux).

### ✅ Step 2: Find the password
Once connected, you'll see a welcome message. Now, run:

```bash
ls
# This lists the files in the current directory. You’ll see a file named:
readme
#Use cat to display the contents:
cat readme
# This will output something like:
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL  # this is not the exact password!!
```
That is your Level 1 password ✅

### 🔐 Password for Level 1
```bash
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
```
You will use this password to log in to Level 1:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

### 📘 Commands Used
Command	Description
- **ssh**:	Connects to a remote machine
- **ls**:	Lists files in a directory
- **cat**:	Displays file contents

### ✅ Summary
- You learned how to connect using SSH.
- You listed the files using ls.
- You read the password file using cat.
- You're ready to move on to Level 1 → Level 2! 🚀