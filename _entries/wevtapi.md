---
Name: wevtapi.dll
Type: Relative Path
Author: Wietze Beukema
Created: 2021-02-27

Vendor: Microsoft
ExpectedLocations:
- "%SYSTEM32%"
VulnerableExecutables:
- Path: "%SYSTEM32%\\gpupdate.exe"
- Path: "%SYSTEM32%\\netsh.exe"
- Path: "%SYSTEM32%\\packageinspector.exe"
- Path: "%SYSTEM32%\\plasrv.exe"
- Path: "%SYSTEM32%\\wecutil.exe"
- Path: "%SYSTEM32%\\wsreset.exe"
  AutoElevate: True

Resources:
- https://wietze.github.io/blog/hijacking-dlls-in-windows
Acknowledgements:
- Name: Wietze
  Twitter: "@wietze"
---