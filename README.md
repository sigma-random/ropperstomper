ropperstomper
=============

Build with llc <http://www.cs.virginia.edu/~lcc-win32/>

Limitations:

* Only supports x86 PE images.
* Doesn't consider linking relocations in gadgets.


```
C:\>ropperstomper.exe c:\Windows\SysWOW64\ntdll.dll
position: 0
...

00044060:     1 MOV DWORD PTR DS:[ESI],EDI | POP EDI | XOR EAX,EAX | POP ESI | POP EBX | POP EBP | RETN 10
