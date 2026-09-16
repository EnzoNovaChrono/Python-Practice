# Chapter 01 Python Basics Notes

## Expressions
### Example: 2 + 4

- Expression are made of two parts
    -   Values (2, 4)
    - Operators (+, -, *)
    
- Expressions **Always** evaluate, in other words, reduce to a single volume


## Math Operators

Python has 7 core math operators. Note the order: Python evaluates
`**` first, then `* / // %`, then `+ -` (standard PEMDAS-style precedence).

| Operator | Operation           | Example  | Evaluates to |
|----------|---------------------|----------|--------------|
| `**`     | Exponentiation      | `2 ** 3` | `8`          |
| `%`      | Modulus / remainder | `22 % 8` | `6`          |
| `//`     | Integer division    | `22 // 8`| `2`          |
| `/`      | Division            | `22 / 8` | `2.75`       |
| `*`      | Multiplication      | `3 * 5`  | `15`         |
| `-`      | Subtraction         | `5 - 2`  | `3`          |
| `+`      | Addition            | `2 + 2`  | `4`          |

### Key things to remember
- **`/` always gives a float** (decimal): `22 / 8` → `2.75`, even if it divides evenly.
- **`//` (integer/floor division) drops the decimal**: `22 // 8` → `2` (not rounded — chopped).
- **`%` (modulus) gives the remainder**: `22 % 8` → `6` (8 goes into 22 twice with 6 left over).
- **`**` is "to the power of"**: `2 ** 3` = 2 × 2 × 2 = `8`.
- The table above is ordered **highest → lowest precedence** (top runs first).


## String Operators

Strings (text) support two math-like operators: `+` and `*`.

| Operator | Operation           | Example              | Evaluates to      |
|----------|---------------------|----------------------|-------------------|
| `+`      | String concatenation| `"Alice" + "Bob"`    | `"AliceBob"`      |
| `+`      | Concatenation w/ space| `"Alice" + " " + "Bob"` | `"Alice Bob"`  |
| `*`      | String replication  | `"Hello" * 5`        | `"HelloHelloHelloHelloHello"` |

### Key things to remember
- **`+` joins strings together** (concatenation). It does NOT add a space —
  `"Alice" + "Bob"` → `"AliceBob"`. To get a space, add one yourself: `"Alice" + " " + "Bob"`.
- **`*` repeats a string** a given number of times (replication):
  `"Hello" * 5` → `"HelloHelloHelloHelloHello"`.
- **Variables can hold strings** and be reused:
  `HW = 'Hello, world!'` then `print(HW)` prints the stored text.
  A variable holding a string works with these operators too: `HW * 5` repeats it 5 times.
- **Quotes:** single `'...'` and double `"..."` both work for strings — just be consistent.
- ⚠️ **`+` only works between two strings.** Mixing a string and a number
  (e.g. `"Alice" + 5`) causes a **TypeError** — you'd have to convert the number
  to a string first with `str(5)`.

  