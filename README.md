Test 1
cd "$env:USERPROFILE\Desktop"

Get-Item .\install.ps1 | Select-Object FullName, Length, LastWriteTime

choco source list


Test 2
Test-Path C:\vm-packages.xml
