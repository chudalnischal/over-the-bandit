
# OverTheWire: Bandit - Level 1

## 🎯 Level Goal

The password for the next level is stored in a file called `-` located in the home directory.

---

## 🧠 What You Learn

- Handling filenames that start with special characters (like `-`)
- Using `cat` and understanding command-line flags
- Quoting and escaping filenames

---

## 🛠️ Solution Strategy

Normally, `cat -` means "read from stdin." But here, the file itself is named `-`, so we need to avoid confusion by explicitly telling the shell it's a file.

### ✅ Correct Command:

```bash
cat ./-
```

Here, `./-` refers to the file `-` in the current directory. The `./` prefix helps avoid confusion with options (flags).

---

## 🔍 Commands Used

- `cat`: To read and display the content of a file
- `ls`: To list files in the directory

---

## 🔑 Output (Password for Level 2)

After running the correct command, you’ll get the password needed to move on to the next level.

---

## 🚀 Moving to the Next Level

Use the password from this level and connect to Level 1 like this:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

---

## 📓 Notes

This level teaches the importance of being careful with filenames and how special characters can change how a command behaves.

