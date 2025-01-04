# Style Guide for Crypto CTF Guide

To maintain consistency and quality across all contributions, please adhere to the following style guide. This guide covers both Markdown documentation and code snippets.

---

## Table of Contents

1. [Markdown Guidelines](#markdown-guidelines)
   - [Headings](#headings)
   - [Lists](#lists)
   - [Links](#links)
   - [Code Blocks](#code-blocks)
   - [Tables](#tables)
2. [Programming Guidelines](#programming-guidelines)
   - [Code Readability](#code-readability)
   - [Commenting](#commenting)
   - [Code Formatting](#code-formatting)
3. [File Organization](#file-organization)
4. [General Tips](#general-tips)

---

## Markdown Guidelines

### Headings

- Use proper heading levels to structure your content:
  - `#` for the title
  - `##` for main sections
  - `###` for subsections
- Avoid skipping heading levels (e.g., don’t jump from `#` to `###`).

Example:
```markdown
# Introduction

## Symmetric Encryption

### Block Ciphers
```

### Lists

- Use `-` or `*` for unordered lists.
- Use `1.`, `2.`, etc., for ordered lists.
- Indent sublists by two spaces.

Example:
```markdown
- Symmetric Cryptography
  - AES
  - DES
- Asymmetric Cryptography
  - RSA
  - ECC
```

### Links

- Use meaningful text for links instead of raw URLs.

Example:
```markdown
[Learn more about AES](https://en.wikipedia.org/wiki/Advanced_Encryption_Standard)
```

### Code Blocks

- Use triple backticks for code blocks.
- Specify the language for syntax highlighting (e.g., `python`, `bash`).
- Keep lines under 80 characters where possible.

Example:
```python
# Python example for calculating modular exponentiation
def mod_exp(base, exp, mod):
    return pow(base, exp, mod)
```

### Tables

- Use `|` to separate columns.
- Align columns for readability.

Example:
```markdown
| Algorithm   | Key Size (bits) | Notes              |
|-------------|-----------------|--------------------|
| AES         | 128, 192, 256  | Symmetric cipher   |
| RSA         | 2048+          | Asymmetric cipher  |
```

---

## Programming Guidelines

### Code Readability

- Use clear and descriptive variable and function names.
- Follow consistent indentation (e.g., 4 spaces for Python).
- Avoid overly complex code; prioritize simplicity.

### Commenting

- Include comments to explain non-obvious logic.
- Use inline comments sparingly; prefer block comments.
- Document the purpose of functions and modules.

Example:
```python
# Calculate the greatest common divisor (GCD)
def gcd(a, b):
    while b:
        a, b = b, a % b
    return a
```

### Code Formatting

- Follow language-specific style guides (e.g., PEP 8 for Python).
- Ensure consistent spacing and alignment.
- Avoid trailing whitespace.

Example (Python PEP 8):
```python
def encrypt(plaintext, key):
    """Encrypts plaintext using a given key."""
    return ''.join(chr(ord(c) ^ key) for c in plaintext)
```

---

## File Organization

- Use meaningful and descriptive file names (e.g., `aes_basics.md`, `rsa_example.py`).
- Group related files in appropriate directories:
  - `/guides` for tutorials
  - `/examples` for code snippets
  - `/resources` for external links or references

---

## General Tips

- Proofread your content for typos and grammar errors.
- Test all code snippets to ensure they work as expected.
- Keep contributions concise and focused.
- Follow the [Code of Conduct](CODE_OF_CONDUCT.md).

Thank you for helping maintain the quality of the Crypto CTF Guide!

