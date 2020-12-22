# Took a byte (Forensics) HTB

Given a zip file , unzipping it we get a text file.
From the title of the challenge, we can determine a byte shift challenge.

Lets try XOR:
Luckily cyberchef has XOR bruteforce.

For the key = ff we get something sensible.

```
Key = ff: PK........×.UN................password.txtUX..ÛDo\.Do\õ...ó.qª62wÌrsÉ.Ì4,÷ªå..PK..MÈþ>........PK....
```

Using the key and then using unzip we get the password.txt

```
password.txt 18 bytes save open_in_browser

HTB{27AjFDkqi1wJ}
```
