# xchmod (Grey Hack)

A Linux-inspired `chmod` implementation for the game **Grey Hack**.

This script supports:
- Numeric permission modes (`000–777`)
- Recursive permission changes (`-R`)
- Helpful CLI flags (`-h`, `-n`)
- Safe permission resets before applying new modes

## Usage

```bash
xchmod <mode> <file/folder>
xchmod -R <mode> <directory/folder>
```
- 0 = ---  (no permissions)
- 1 = --x  (execute only)
- 2 = -w-  (write only)
- 3 = -wx  (write + execute)
- 4 = r--  (read only)
- 5 = r-x  (read + execute)
- 6 = rw-  (read + write)
- 7 = rwx  (read + write + execute)

Each digit applies to a permission group:

- First digit  -> user (owner)
- Second digit -> group
- Third digit  -> others
