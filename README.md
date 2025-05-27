````markdown
# Regex Sandbox

A simple web app that lets you test regular expressions against input strings with live highlighting of matches.

---

## Overview

This Regex Sandbox allows users to:

- Enter a regex pattern.
- Specify optional flags (`i` for case-insensitive, `g` for global).
- Input a test string.
- Test the regex against the string.
- See all matches highlighted inside the test string.
- View a list of matched substrings.
- Receive feedback when there are no matches.

The app is built with HTML, CSS, and JavaScript — no external dependencies.

---

## Features

- Supports `i` and `g` flags for regex matching.
- Highlights matched substrings inside the editable test string.
- Displays matched results separated by commas.
- Shows `no match` message if nothing matches.
- Handles invalid regex patterns gracefully.
- Prevents HTML injection by escaping user input.

---

## Usage

1. Enter your regex pattern (without slashes) into the **Regex Pattern** input.
2. Check the flags (`i` for case-insensitive, `g` for global) as needed.
3. Type or paste your test string in the editable **Test String** area.
4. Click the **Test Regex** button.
5. See matched text highlighted and the matched results listed below.

---

## Code Highlights

- Uses `RegExp` constructor dynamically with flags.
- Supports both global and single match modes:
  - Uses `String.matchAll()` if global flag is set.
  - Uses `RegExp.exec()` for a single match otherwise.
- Highlights matches by wrapping them in `<span class="highlight">` elements.
- Escapes HTML entities in input and output to ensure security and proper rendering.

---

## Installation

Simply clone or download the repository and open `index.html` in a modern browser.

```bash
git clone https://github.com/yourusername/regex-sandbox.git
cd regex-sandbox
open index.html
```

---

## Future Improvements

* Add support for more regex flags (`m`, `s`, `u`, `y`).
* Provide real-time matching as the user types.
* Save regex history for quick access.
* Add regex syntax helper or autocomplete.
* Support replace functionality.

---

## License

This project is open-source and free to use under the MIT License.

---

## Author

Jordan Leturgez
---

Feel free to contribute or suggest features!

```
