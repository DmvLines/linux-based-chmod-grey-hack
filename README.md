# xchmod (Grey Hack)

A Linux-inspired `chmod` implementation for the game **Grey Hack**.

This script supports:
- Numeric permission modes (`000–777`)
- Recursive permission changes (`-R`)
- Helpful CLI flags (`-h`, `-n`)
- Safe permission resets before applying new modes

## Usage

```bash
xchmod <mode> <file>
xchmod -R <mode> <directory>
