# caesar-cipher

A simple Python implementation of the Caesar cipher, one of the oldest
encryption techniques. Each letter is shifted a fixed number of places
along the alphabet.

## Features
- Encrypt and decrypt text with a shift from 1 to 25
- Preserves uppercase and lowercase letters
- Leaves spaces, numbers, and punctuation unchanged
- Validates the shift value

## Usage

```python
from caesar import encrypt, decrypt

encrypted = encrypt('freeCodeCamp', 3)
print(encrypted)                # iuhhFrghFdps
print(decrypt(encrypted, 3))    # freeCodeCamp
```

Or run the file directly:

```
python caesar.py
```

## How it works
The program builds a shifted copy of the alphabet and uses Python's
`str.maketrans()` and `translate()` to swap each letter for its shifted
counterpart. Decryption uses the same method with the shift reversed.

## Example

| Input          | Shift | Output         |
|----------------|-------|----------------|
| freeCodeCamp   | 3     | iuhhFrghFdps   |
| Hello, World!  | 5     | Mjqqt, Btwqi!  |

## Ideas for improvement
- Brute-force mode that tries all 25 shifts
- Support for shifts outside 1-25
- Unit tests
- A Java version

## Author
Sadew Chamika