# MSIX Package with PWA and Win32 App

This is an MSIX package that includes:

- A Progressive Web App (PWA) manually packaged into a UWP using WebView2:  
  [WebView2 for WinUI 2](https://learn.microsoft.com/en-us/microsoft-edge/webview2/get-started/winui2)
- A portable Win32 application

## Running the Project

Run the solution in **Release mode** using Visual Studio, or package it manually:

1. Right-click the UWP project within the solution
2. Select **Publish > Create App Packages**
3. Choose the desired architectures

## Troubleshooting

If you encounter issues running the project, remove previously installed versions of the package by running the following PowerShell command **as Administrator**:

```powershell
Get-AppxPackage -AllUsers _ManualPackagePWA_ | Remove-AppxPackage -AllUsers
```
