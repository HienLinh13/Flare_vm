Test 1
cd "$env:USERPROFILE\Desktop"

Get-Item .\install.ps1 | Select-Object FullName, Length, LastWriteTime

choco source list


Test 2
Test-Path C:\vm-packages.xml

Test 3
@"
<?xml version="1.0" encoding="utf-8"?>
<packages>
</packages>
"@ | Out-File -FilePath "C:\vm-packages.xml" -Encoding utf8

Test 4 
cd $env:USERPROFILE\Desktop
powershell -ExecutionPolicy Bypass .\install.ps1
