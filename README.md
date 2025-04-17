# ffuf-simple-script
Simple ffuf tool project with bash scripting
# 🔍 FFUF Automation Script

A simple interactive Bash script to automate common fuzzing tasks using [ffuf](https://github.com/ffuf/ffuf).

Created with ❤️ by **EGDarko**

---

## 📜 Description

This script provides a menu-driven interface for using `ffuf` to perform various types of fuzzing tasks like:

- Directory fuzzing
- Subdomain fuzzing
- File extension fuzzing
- Extension list fuzzing
- Recursive directory fuzzing

Just run the script, input your target URL, wordlist path, and number of threads — then pick a template!

---

## 🧰 Requirements

- **Linux or macOS terminal**
- [ffuf](https://github.com/ffuf/ffuf) must be installed and available in your `$PATH`
- A valid **wordlist** for fuzzing (e.g., from [SecLists](https://github.com/danielmiessler/SecLists))

---

## 🚀 Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/EGDarko/ffuf-bash-script.git
   cd ffuf-bash-script
