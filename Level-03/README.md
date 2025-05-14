# OverTheWire: Bandit – Level 2 → Level 3

## 🧠 Objective

The goal of this level is to find the password for the next level, which is **stored in a file with spaces in its name**.

---

## 🔐 Login Information

- **Username:** `bandit2`
- **Hostname:** `bandit.labs.overthewire.org`
- **Port:** `2220`
- **Password:** `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi` (demo password)

---

## 🧪 Steps to Solve Level 2

### ✅ Step 1: Connect to the server

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

Enter the password when prompted: `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi`

---

### ✅ Step 2: List the files

```bash
ls
```

You will see a file named like:

```
spaces in this filename
```

> ⚠️ Since the filename contains **spaces**, you must handle it carefully in the command line.

---

### ✅ Step 3: Read the file with spaces in its name

You have two safe ways to do this:

**Option 1: Use quotes**
```bash
cat "spaces in this filename"
```

**Option 2: Escape spaces with backslashes**
```bash
cat spaces\ in\ this\ filename
```

You will get an output like:

```bash 
aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG # demo password
```

That is your **Level 3 password** ✅
To connect to the next level:

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```
---

## 📘 Commands Used

| Command                                | Description                                |
|----------------------------------------|--------------------------------------------|
| `ls`                                   | List directory contents                    |
| `cat "filename with spaces"`           | Safe way to read files with spaces         |
| `cat filename\ with\ escaped\ spaces`| Alternate way using escape characters      |


## ✅ Summary

- You learned how to handle filenames that contain **spaces**.
- You used quotes or escape characters to safely read such files.

Now you're ready for **Level 3 → Level 4**! 🚀
