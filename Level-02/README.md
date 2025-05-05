
# OverTheWire: Bandit - Level 2

## 🎯 Level Goal

The password for the next level is stored in a file called `spaces in this filename` located in the home directory.

---

## 🧠 What You Learn

- Handling filenames with spaces
- Using quotes or escape characters in the command line

---

## 🛠️ Solution Strategy

Filenames with spaces need to be wrapped in quotes or escaped with backslashes.

### ✅ Correct Commands:

```bash
cat "spaces in this filename"
```

OR

```bash
cat spaces\ in\ this\ filename
```

---

## 🔍 Commands Used

- `cat`: To read file content
- `ls`: To check the file is there

---

## 🔑 Output (Password for Level 3)

After using one of the commands above, you’ll see the password for Level 3.

---

## 🚀 Moving to the Next Level

Use the password you just found and connect to Level 2:

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

---

## 📓 Notes

This level emphasizes careful handling of file names that contain spaces. In Linux, spaces are treated as argument separators unless quoted or escaped.

