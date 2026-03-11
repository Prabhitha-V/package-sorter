# Package Sorter

A dispatch sorting function for a robotic automation system that routes packages to the correct stack based on their dimensions and mass.

## Logic

| Condition | Stack |
|---|---|
| Neither bulky nor heavy | STANDARD |
| Bulky or heavy (not both) | SPECIAL |
| Both bulky and heavy | REJECTED |

**Bulky:** volume ≥ 1,000,000 cm³ or any single dimension ≥ 150 cm  
**Heavy:** mass ≥ 20 kg

## Usage
```bash
# Run smoke test
python package_sorter.py

# Run full test suite
pytest package_sorter.py -v
```

## Requirements

Python 3.7+ and pytest:
```bash
pip install pytest
```
