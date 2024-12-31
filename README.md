# B64Reversed-Math
Encodes each line to base64, reverts them & builds the decryption. Afterwards obfuscates all reverted b64 keys with math techniques. Also uses MBA obfuscated commands/strings ;D
As this is annoying/hard to reverse, don't obfuscate any harmful code with it...

![b64pre](https://github.com/5Noxi/B64Reversed-Math/blob/main/NV-RevMath1.png?raw=true)
![b64pre2](https://github.com/5Noxi/B64Reversed-Math/blob/main/NV-RevMath2.png?raw=true)
### Before
![before](https://github.com/5Noxi/B64Reversed-Math/blob/main/Before.png?raw=true) 
### After
![after](https://github.com/5Noxi/B64Reversed-Math/blob/main/After.png?raw=true)

## Discord Server 
- https://discord.gg/E2ybG4j9jU

## Features
- Base64 **reversal** and **string manipulation**
- **Mathematical obfuscation** using various techniques to randomize **all reversed b64 lines**
- Obfuscates **all** commands with randomized MBA presets
- **Extremely annoying & hard to reverse ;D** - tell me, if you're able to 

## Example for MBA obfuscated `frombase64` command
```
([char](((55 -Band 6708) + (55 -Bor 6708) + 1326 - 8019))+[char]((-3766 - 6100 + 9349 + 599))+[char](((-4234 -Band 3291) + (-4234 -Bor 3291) - 8845 + 9867))+[char](((-8050 -Band 6192) + (-8050 -Bor 6192) + 4340 - 2405))+[char](((-14861 -Band 7409) + (-14861 -Bor 7409) - 271 + 7789))+[char]((5715 - 8922 + 1287 + 1985))+[char](((6544 -Band 7874) + (6544 -Bor 7874) - 6162 - 8173))+[char](((-1209 -Band 6187) + (-1209 -Bor 6187) - 276 - 4633))+[char]((2515 - 3825 - 6060 + 7424))+[char](((5333 -Band 1018) + (5333 -Bor 1018) - 7498 + 1199))+[char](((-8337 -Band 4462) + (-8337 -Bor 4462) + 188 + 3770))+[char]((-300 - 411 - 1962 + 2757))+[char](((-9604 -Band 4993) + (-9604 -Bor 4993) + 6600 - 1907))+[char](((-11046 -Band 2272) + (-11046 -Bor 2272) + 9314 - 435))+[char](((967 -Band 8319) + (967 -Bor 8319) - 7360 - 1816))+[char](((3041 -Band 1800) + (3041 -Bor 1800) - 9458 + 4720)))
```

## User-friendly explanation
1. Gets b64 format of each line, for example `Tm92ZXJzZQ==`
2. Reverts it to `==QZzJXZ29mT`
3. Builds decryption command for it
```
[syStem.texT.encoDing]::utF8.GeTString([syStem.COnvert]::frombase64STRING(-Join(...)
```
4. Obfuscates **all** commands with MBA (as shown above)
5. Obfuscates all lines, which are showing the b64 reverts with mathematical techniques

## Usage
`nvi` -> Input

`nvo` -> Output

`. \NV-Rev64.Math.ps1;reversed -nvi "\Test.ps1" -nvo "\Reversed.ps1"`

## Warning
You probably can't encrypt **big files** with it! If you want to know how to use it for whole files, join the discord server.
Also: **Don't be a kiddo**, I uploaded the script *open source and for free*, stealing it now would be **unbelievable** ;D *(sad)* 

## Disclaimer 
**I'm not responsible for any misuse of this tool!**
