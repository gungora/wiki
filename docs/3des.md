---
tags:
  -  Encryption
  -  Anti-Forensics
---
**3DES** or **Triple DES** is a block cipher formed by using the Data
Encryption Standard ([des](des.md) cipher three times.

3DES is typically implemented as ENCRYPT(block,K1), DECRYPT(block,K2),
ENCRYPT(block,K3). This way, if you set K1==K2 it's backwards compatible
with single-key DES with K3. It's pretty cool, but perhaps less useful
today than it was when 3DES was first brought out.

## External Links

- [Wikipedia: 3DES](http://en.wikipedia.org/wiki/Triple_DES)

<!-- -->

- [Using 3DES for Hard Drive Encryption](http://secude.com/htm/805/en/White_Paper_Section%3A_Full_Disk_Encryption.htm)

