<!-- [60 Points] Digital Cube -->
# [60 Points] Digital Cube

...Strathmore leaned forward and rotated his monitor toward Susan. The screen was black except for a small, white text box blinking in the middle. TIME ELAPSED: 50:50"
TRANSLTR, the single best crypto-machine, could not crack this code. Maybe you can...

[Downloads](./digitalcube.zip)  
Zip Password: hackthebox sha256: ecd005e153f20cb1a057719345fcc67d897c107ee9df1521edf10549aee09fb7

<!-- Exploit: -->
## Exploit:

Extract the files from given zip file.

A text file containing 1s and 0s is given. [digitalcube.txt](./digitalcube.txt)

I've tried binary decoding and morse but it didn't work.
Then tried binary to img decoding and it gave a qrcode.

![decode-image.png](./decode-image.png)

Use [Zbarimg](https://wiki.bi0s.in/steganography/zbarimg/) tool to analyse the QR coded.
```
$ zbarimg dcode-image.png
```
This gives us the flag.

<!-- Flag: -->
## Flag:
```
HTB{QR_!snt_d34d}
```




