# Write-a-Python-program-to-remove-leading-zeros-from-an-IP-address
import re

def is_allowed_specific_char(string):
    charRe = re.compile(r'[^a-zA-Z0-9]')
    string = charRe.search(string)
    return not bool(string)

print(is_allowed_specific_char("ABCDEFabcdef123450"))
print(is_allowed_specific_char("*&%@#!}{"))

output
.

======================= RESTART: C:/Python3.14/PYTHON.py =======================
True
False

