# Minishell

_As beautiful as a shell_

## 📝 Summary

This project is about creating a simple shell. Yes, your very own little Bash.
You will gain extensive knowledge about processes and file descriptors.

## 📁 Project Structure

- Language: C (following the **Norm**)
- External Functions: `readline`, `fork`, `execve`, `pipe`, `dup2`, etc.
- Authorized Library: **libft**

## ✅ Mandatory Features

- Prompt display while waiting for user input
- Command history (via `readline`)
- Executable search (via `$PATH`, relative or absolute path)
- Signal handling with a **single** global variable
- Handling of:
  - Single quotes `'` (no interpretation of meta-characters)
  - Double quotes `"` (except `$` expansion)
  - Redirections: `<`, `>`, `<<`, `>>`
  - Pipes `|`
  - Environment variables `$VAR`, `$?`
- Interactive controls:
  - `ctrl-C`: displays new prompt
  - `ctrl-D`: exits shell
  - `ctrl-\`: does nothing
- Built-in commands:
  - `echo [-n]`
  - `cd [path]`
  - `pwd`
  - `export`
  - `unset`
  - `env`
  - `exit`

## ⚙️ Compilation

```bash
make
```

Makefile rules required: `all`, `clean`, `fclean`, `re`, `bonus`

## 📌 Notes

- No memory leaks are allowed (excluding `readline()`)
- Unclosed quotes and unsupported special characters are **not** interpreted
- Always refer to Bash for behaviour in case of doubts

## 📂 Submission

Submit only through the assigned Git repository. Ensure all file names and structure follow the subject's instructions.

---

> "With Minishell, you’ll travel back in time and experience the challenges developers faced before Windows existed." 🕰️
