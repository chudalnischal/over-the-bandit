# OverTheWire: Bandit – Level 3 → Level 4

## 🧠 Objective

The goal of this level is to find the password for the next level, which is **stored in a hidden file inside a directory named `inhere`**.

## 🔐 Login Information

- **Username:** `bandit3`
- **Hostname:** `bandit.labs.overthewire.org`
- **Port:** `2220`
- **Password:** `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG` (demo password)
---

## 🧪 Steps to Solve Level 3

### ✅ Step 1: Connect to the server

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```

Enter the password when prompted: `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG`

---

### ✅ Step 2: Navigate into the directory

```bash
cd inhere
```

List all files including hidden ones using:

```bash
ls -a
```

You’ll see something like:

```
.  ..  .hidden
```

> 🕵️ Files that start with a `.` are hidden and won’t show up with regular `ls`. That's why we used `-a` (all).

---

### ✅ Step 3: Read the hidden file

```bash
cat .hidden
```

This will display the password for the next level, such as:

```bash 
2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe # demo password
```

That is your **Level 4 password** ✅

To move on to the next level:

```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```
--- 

## 📘 Commands Used

| Command       | Description                                 |
|---------------|---------------------------------------------|
| `cd`          | Change directory                            |
| `ls -a`       | List all files including hidden ones        |
| `cat .hidden` | Read a hidden file                          |

## ✅ Summary

- You found and accessed a hidden file using `ls -a`.
- You used `cat` to read its content.
- You retrieved the password for the next level.

You're now ready for **Level 4 → Level 5**! 🔓
