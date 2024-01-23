```markdown
# Terminal Shortcuts

- **CTRL + A:** Move cursor to the beginning of the command line.
- **CTRL + E:** Move cursor to the end of the command line.

- **ALT + F:** Move one word forward.
- **ALT + B:** Move one word backward.

- **CTRL + U:** Erase everything from the current position to the beginning of the line.
- **CTRL + K:** Erase everything from the current position to the end of the line.

# Command Chaining
- `;`: Executes commands one after another regardless of whether the previous command fails.
- `&&`: Stops if a command fails.

Example:
```bash
git add . && git commit -m "my commit" && git push origin main
```

# Command History
- **Up Arrow:** Cycle through the list of previous commands.
- **CTRL + R:** Begin typing a command, press enter if it pulls up the one you entered previously.
- **history, !593** Type `history`, then enter the corresponding command with `!` in front (e.g., `!593`).


# Instead of clear command

- **Ctrl + L** - Shortcut for typing clear and then enter.
```