# OverTheWire: Bandit – Level 1 → Level 2

## 🧠 Objective

The goal of this level is to find the password for the next level, which is **stored in a file named `-`** (just a hyphen).

---

## 🔐 Login Information

- **Username:** `bandit1`
- **Hostname:** `bandit.labs.overthewire.org`
- **Port:** `2220`
- **Password:** `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`  (demo password)

---

## 🧪 Steps to Solve Level 1

### ✅ Step 1: Connect to the server

Use the following SSH command:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```
When prompted, enter the password: `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`

---

### ✅ Step 2: List files

```bash
ls
```

You will see a file named:

```
-
```

> ⚠️ Special character alert: The hyphen `-` is interpreted as an **option flag** in many commands. So you must handle it carefully.

---

### ✅ Step 3: Read the file named `-`

To avoid confusion with command-line options, you can use:

```bash
cat ./-
```

This forces the shell to treat `-` as a file name instead of a flag.

You will see an output like:

```bash
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi # demo password
```

That is your **Level 2 password** ✅

---

## 🔐 Password for Level 2

```bash
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi
```

To log in to the next level:

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

---

## 📘 Commands Used

| Command   | Description                            |
|-----------|----------------------------------------|
| `ls`      | Lists files in the current directory   |
| `cat`     | Displays the content of a file         |
| `./-`     | Access the file named `-` using relative path |

---

## ✅ Summary

- You learned how to read files with special names like `-`.
- You used relative path (`./`) to avoid command interpretation issues.

You're now ready for **Level 2 → Level 3**! 🎉
