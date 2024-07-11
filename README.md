# Hashmash

Hashmash is a simple web application that takes a string input and an optional salt string, then provides descriptive statistics about the input and calculates various hash values. The application updates the statistics and hashes in real-time as the input changes.

## Try it out here:
[hashmash](https://deftio.github.io/hashmash/index.html)

## Features

- Displays descriptive statistics for the input string:
  - Characters
  - Words
  - Numbers
  - Uppercase Letters
  - Lowercase Letters
  - Symbols
  - Spaces/Tabs
  - Non-ASCII Characters
- Calculates the following hashes for the input string:
  - 32-bit Checksum
  - 64-bit Checksum
  - 16-bit CRC
  - 32-bit CRC
  - 64-bit CRC
  - MD5
  - SHA1
  - SHA224
  - SHA256
  - Hex ASCII
- Allows the user to add an optional salt to the input string.
- Allows the user to specify a prefix for the hex hash values.
- The application is responsive and adjusts to fit horizontally in the viewport.

## Installation

No installation is required. Simply open the `index.html` file in your web browser.

## Usage

1. Open `index.html` in your web browser.
2. Enter your input string in the provided text area.
3. Optionally, enter a salt string in the salt input field.
4. Optionally, enter a prefix string in the prefix input field (default is `Mi$0`).
5. The descriptive statistics and hash values will update in real-time as you type.

## Code Overview

### HTML Structure

- A text area for the input string.
- An input field for the optional salt string.
- An input field for the optional prefix string.
- A div to display the descriptive statistics.
- A table to display the hash values.

### JavaScript Functions

- `updateStatsAndHashes()`: Updates the descriptive statistics and hash values whenever the input string, salt, or prefix changes.
- `getStats(str)`: Returns an object containing various statistics for the input string.
- `getHashes(str, prefixValue)`: Returns an array of hash objects for the input string.
- `displayStats(stats)`: Displays the descriptive statistics in a table format.
- `displayHashes(hashes)`: Displays the hash values in a table format.
- `toHexASCII(str)`, `toChecksum32(str)`, `toChecksum64(str)`, `toCRC16(str)`, `toCRC32(str)`, `toCRC64(str)`: Functions for calculating various hash values.

### Dependencies

- [CryptoJS](https://cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/crypto-js.min.js): A JavaScript library for performing cryptographic operations.



## License

This project is licensed under the BSD-2 License. See the LICENSE file for details.
