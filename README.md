# B64Reversed-Math-Obfuscator
Obfuscates a random of about of `2-6`**lines** with b64, **reverts** them & builds the decoding part. Afterwards obfuscates all reverted B64 commands with **math techniques**.

**Preview:**
![b64pre](https://github.com/5Noxi/B64Reversed-Math/blob/main/rev1.png?raw=true)
![b64pre2](https://github.com/5Noxi/B64Reversed-Math/blob/main/rev2.png?raw=true)
### Before
![before](https://github.com/5Noxi/B64Reversed-Math/blob/main/before.png?raw=true) 
### After
![after](https://github.com/5Noxi/B64Reversed-Math/blob/main/after.png?raw=true)

## Features:
- Base64 **reversal** and **string obfuscation**
  - Creates obfuscated vars, using random letters from the "**Arabic, Chinese, Japanese, Russian, Greek, Korean**" alphabets
  - Each var has a random length of `32-64` chars from the preset & a predefined string
  -  Takes randomly a amount of `2-6` lines
- **Math obfuscation** using various techniques to randomize **all reversed b64 lines** - uses numbers from `1000000` up to `999999999` (max)
- Obfuscates **all** commands with randomized presets
- And much more...

#### Example of obfuscated `frombase64` command:
```ps
([char](((55 -Band 6708) + (55 -Bor 6708) + 1326 - 8019))+[char]((-3766 - 6100 + 9349 + 599))+[char](((-4234 -Band 3291) + (-4234 -Bor 3291) - 8845 + 9867))+[char](((-8050 -Band 6192) + (-8050 -Bor 6192) + 4340 - 2405))+[char](((-14861 -Band 7409) + (-14861 -Bor 7409) - 271 + 7789))+[char]((5715 - 8922 + 1287 + 1985))+[char](((6544 -Band 7874) + (6544 -Bor 7874) - 6162 - 8173))+[char](((-1209 -Band 6187) + (-1209 -Bor 6187) - 276 - 4633))+[char]((2515 - 3825 - 6060 + 7424))+[char](((5333 -Band 1018) + (5333 -Bor 1018) - 7498 + 1199))+[char](((-8337 -Band 4462) + (-8337 -Bor 4462) + 188 + 3770))+[char]((-300 - 411 - 1962 + 2757))+[char](((-9604 -Band 4993) + (-9604 -Bor 4993) + 6600 - 1907))+[char](((-11046 -Band 2272) + (-11046 -Bor 2272) + 9314 - 435))+[char](((967 -Band 8319) + (967 -Bor 8319) - 7360 - 1816))+[char](((3041 -Band 1800) + (3041 -Bor 1800) - 9458 + 4720)))
```

#### Obfuscated var example:
```ps
$вογιNوϖoχtσnξOxιΔXψнгzIΞqF理БШフエ些سеヲ有вογιNوϖoχtσnξOxιΔXψ
```

#### User friendly explanation:
1. Gets b64 format of each line, for example `Tm92ZXJzZQ==`
2. Reverts it to `==QZzJXZ29mT`
3. Builds decryption command for it (including reverse part):
```ps
[syStem.texT.encoDing]::utF8.GeTString([syStem.COnvert]::frombase64STRING(-Join(...)
```
4. Obfuscates **all** commands with MBA (as shown above)
5. Obfuscates all lines, which are showing the b64 reverts with mathematical techniques

## Usage
`nvi` -> Input

`nvo` -> Output

`. \NV-Rev64.Math.ps1;reversed -nvi "\Test.ps1" -nvo "\Reversed.ps1"`

## Warning
You probably can't obfuscate **complicated code** with it! **Don't be a kiddo**, I uploaded the script *open source and for free*, stealing it now would be **unbelieveable** sad. **I'm not responsible for any misuse of this tool!**

## Discord Server 
- https://discord.gg/E2ybG4j9jU
