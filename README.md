# seed-generator

Standalone English BIP39 recovery phrase generator.
Available as a Python terminal application and a self-contained HTML page.

## Features

- 24 English words from 256 bits of cryptographic entropy.
- Python secrets and browser Web Crypto for secure randomness.
- BIP39 checksum validation and public-vector self-tests.
- Embedded official English wordlist.
- No external dependencies or network requests.
- Responsive HTML interface with show/hide, copy and clear controls.
- Numbered Python terminal layout with optional colors.

## Usage

Python 3.8 or newer, in an interactive terminal:

    python3 seed-generator.py

Run public self-tests without generating secrets:

    python3 seed-generator.py --self-test

Disable terminal colors:

    python3 seed-generator.py --no-color

For HTML, download seed-generator.html and open it in a modern browser.
Generation is blocked if Web Crypto is unavailable.

## Security

Anyone with the recovery phrase can access the associated wallet.
Use a trusted device, preferably offline. Write down the words in order
and store them securely. Avoid screenshots, email and cloud storage.

Clipboard managers, synchronization and terminal scrollback may retain
copies. Hiding words does not erase them from memory. Secure memory
erasure cannot be guaranteed.

Checksum validation confirms the BIP39 format, not device security or
compatibility with every wallet. For significant funds, prefer generating
the recovery phrase directly on a hardware wallet.

Earlier versions used random generators unsuitable for cryptographic
secrets. If used for a funded wallet, migrate to a wallet with a newly
generated recovery phrase.

## Signing key

The current public signing key is included in pub_key.asc.

Fingerprint:
37A4179C7B80C50304231586C97F93FDD23170E8

This replaces the previous key, whose private part is no longer available.
Never commit private keys or generated recovery phrases.

## Author

vinacc — va@vinacc.eu

## License

MIT License.
