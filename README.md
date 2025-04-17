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
   git clone https://github.com/EGDarko/ffuf-simple-script.git
   cd ffuf-bash-script
   ```

2. Make the script executable:

   ```bash
   chmod +x ffuf-script.sh
   ```

3. Run the script:

   ```bash
   ./ffuf-script.sh
   ```

4. Follow the prompts:

   - Enter the target URL with `FUZZ` as the injection point.
   - Provide the path to your wordlist.
   - Set the number of threads.
   - Choose the fuzzing type from the menu.

---

## 📋 Example

```text
========= FFUF Script =========
        By: EGDarko

Enter URL with FUZZ in the place you want to inject payload:
  For DIR fuzzing     => Example: http://example.com/FUZZ
  For Subdomain fuzzing => Example: example.com
  For Extension fuzzing => Example: https://example.com/index.FUZZ

URL: http://example.com/FUZZ
Enter Wordlist path: /usr/share/seclists/Discovery/Web-Content/common.txt
Enter number of threads: 50

Select a template:
1) Basic directory fuzzing
2) Subdomain fuzzing
3) File extension fuzzing (.php)
4) Extension fuzzing [Use extensions wordlist like: php,html,js]
5) Directory fuzzing with -recursion

Enter your choice (1-5): 1
```

---

## 🧠 Notes

- Make sure the target URL contains the word `FUZZ` for the injection point.
- Supports colorful terminal output for better readability.
- Easily customizable for more fuzzing patterns.

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙌 Credits

- [ffuf](https://github.com/ffuf/ffuf) by **@ffuf**
- Script by **EGDarko**
