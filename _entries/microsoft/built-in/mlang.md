---
Name: mlang.dll
Author: Wietze Beukema
Created: 2021-02-27
Vendor: Microsoft
ExpectedLocations:
- '%SYSTEM32%'
- '%SYSWOW64%'
VulnerableExecutables:
- Path: '%SYSTEM32%\calc.exe'
  Type: Sideloading
- Path: '%SYSTEM32%\computerdefaults.exe'
  Type: Sideloading
  AutoElevate: true
- Path: '%SYSTEM32%\fodhelper.exe'
  Type: Sideloading
  AutoElevate: true
- Path: '%SYSTEM32%\ie4uinit.exe'
  Type: Sideloading
- Path: '%PROGRAMFILES%\Microsoft Office\root\Office%VERSION%\excel.exe'
  Type: Environment Variable
  Variable: SYSTEMROOT
  Condition: Tested against Microsoft Office 2021
Resources:
- https://wietze.github.io/blog/hijacking-dlls-in-windows
Acknowledgements:
- Name: Wietze
  Twitter: '@wietze'
---
