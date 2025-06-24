This is a msix package including a PWA and a a portable win32 app

run it in release mode using visual studio.

if you are facing any issues executing the project, run this with admin rights:

`Get-AppxPackage -AllUsers _ManualPackagePWA_ | Remove-AppxPackage -AllUsers`
