# 🐚 minishell

**minishell** is a minimal Unix shell implemented in C as part of the 42 curriculum. It replicates core features of Bash, including command parsing, execution, environment variable handling, and redirections. This repository contains the mandatory part of the project and optionally includes bonus features.

---

## 💻 How It Works

- Displays a prompt and waits for user input.
- Parses and executes commands with arguments.
- Handles built-in commands like `cd`, `echo`, and `export`.
- Supports piping, redirections, and environment variables.
- Implements signal handling to behave like Bash.

---

## 📋 Features

### **Mandatory**
- Custom prompt and command input via `readline`.
- Built-in commands:
  - `echo [-n]`
  - `cd [path]`
  - `pwd`
  - `export`
  - `unset`
  - `env`
  - `exit`
- Redirections:
  - Input `<`
  - Output `>`
  - Append `>>`
  - Here-document `<<`
- Piping (`|`) between commands.
- Environment variable expansion (`$VAR`, `$?`).
- Proper signal handling (`ctrl-C`, `ctrl-D`, `ctrl-\`).

---

## 🚀 Getting Started

### Prerequisites
- Unix-like OS (Linux or macOS).
- GNU Readline library.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/teu-username/minishell.git
   cd minishell
   ```

2. Compile the project:
   ```bash
   make
   ```

3. Run the shell:
   ```bash
   ./minishell
   ```

---

## 📂 File Structure

```
minishell/
├── include/            # Header files
├── src/                # Source code
│   ├── main.c          # Entry point
│   ├── exec/           # Command execution
│   ├── parser/         # Parsing logic
│   ├── builtins/       # Built-in commands
│   ├── signals/        # Signal handling
│   ├── env/            # Environment management
├── libft/              # Custom standard library (if used)
├── Makefile            # Build instructions
└── README.md           # Project documentation
```

---

## 🛠️ Built With

- GNU Readline - For interactive input.
- C (following the Norm coding standard).

---

## 📖 Future Improvements

- Advanced wildcard and globbing support.
- Job control (`fg`, `bg`, `jobs`).
- History persistence across sessions.

---

## ✨ Acknowledgments

This project is part of the 42 Network curriculum. Grateful to the 42 community for collaboration and support.

---

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for details.
