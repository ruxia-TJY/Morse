# Morse

A simple package for morse decode and encode.

```python
from Morse import morse

M = morse.Morse()

print(M.encode('morse'))
# ————/——————/.——./.../.
print(M.decode('————/——————/.——./.../.'))
# MORSE
M.isLower = True
print(M.decode('————/——————/.——./.../.'))
# morse

M.Separator = '?'
print(M.encode('morse'))
# ————?——————?.——.?...?.

M.dot = '<'
M.dash = '>'
print(M.encode('morse'))
# >>/>>>/<></<<</<
```