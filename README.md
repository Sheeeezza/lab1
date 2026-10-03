 Celsius to Fahrenheit Converter (Hand vs AI)
## Description
The same Celsius-to-Fahrenheit converter built twice: once by hand and
once with an AI assistant, then compared honestly.

## How to Run
```
python lab1.py
```
Enter a number when asked, e.g. `100`. Output: `100.0C = 212.0F`.
Entering non-numeric input prints `Please enter a number.`

## Files
- `hand_written.py`: hand-written version (branch `main`)
- `ai_assisted.py`: AI-assisted version (branch `ai-build`)

## What I Did
1. **Hand-built version:** first draft gave wrong answers because of
   integer-style division. Found by testing a known value (100C = 212F).
   Fixed with `c * 9 / 5 + 32`.
2. **AI-assisted version:** used true division, a type hint, a docstring,
   and `try/except` around `input()`.
3. **Comparison:** the AI did not just get lucky, it defaulted to float
   division and input checking.

## Evidence
- Commit history: `<paste output of git log --format='%h %ad %s' --date=iso>`
- Python version: `<paste output of python -VV>`
- Prompt used: `<paste exact prompt>`
- Suggestion I rejected: `<paste>`; why it was wrong: `<one sentence>`

## Findings
- **Where AI helped:** input validation and float division without being asked.
- **Where it cost time:** checking its extra code (docstring, hints).
- **Limitation:** it only catches `ValueError`, so an EOF error on `input()`
  would still crash it.



<img width="576" height="627" alt="LAB1" src="https://github.com/user-attachments/assets/064bf363-7857-4979-bf13-2be4daaab488" />

## Take-Home
Tip splitter built twice (`split_tip` and `split_tip_safe`). The safe
version rejects negative bills and `people < 1`.
