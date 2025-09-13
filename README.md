# Base64 Reversal & Character Obfuscation

Encodes with B64, reverts them & builds the decoding part. Afterwards obfuscates all reverted B64 commands with character obfuscation.  It detects the correct line amount per encoding string automatically. Variable names and everything else has either a obfuscated preset or gets created with random caps. `Input File` is mandatory, if the `Output File` path isn't set, it'll use the current file name and adds `NV-`.

Preview:

https://github.com/user-attachments/assets/2b876ac2-29f6-4321-a372-91f595ae02ae

1. Encodes the string to B64, e.g. `Tm92ZXJzZQ==`
2. Reverts it to `==QZzJXZ29mT`
3. Builds decoding command for it (including reverse part):
```ps
[system.text.encoding]::utf8.getstring([system.convert]::frombase64string(-join(...)
```
4. Character obfuscation of all lines, which include the encoded string

The string depends on if the line starts a code block or not:
```ps
$bracket = if ($line -match '\{') { '{' } else { '(' }
$closing = if ($bracket -eq '{') { '}' } else { ')' }
```
It tracks nested brackets and uses the whole block as string, otherwise each line get's encoded on it's own.

## GUI Buttons
| Button             | Description                                                                                              |
|--------------------|----------------------------------------------------------------------------------------------------------|
| `Detailed Logging` | Displays the block start/end or line.                                                                    |
| `Add Dead Branches`| Adds dead `if` blocks, with each `FromBase64String` method getting its own dedicated block.               |
| `One Invoke`       | Fastest start and lowest security (decodes everything at once using a single `ToBase64String` operation) |
