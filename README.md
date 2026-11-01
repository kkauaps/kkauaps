# BareWin

**Uninstaller + Debloat for Windows 10/11** · **Desinstalador + Debloat para Windows 10/11**

Portable, self-contained `BareWin.exe` (no .NET install needed) or MSI installer.

## Features
- Lists apps from the registry **and** loose program folders (e.g. Ollama in `%LOCALAPPDATA%\Programs`)
- App icon, install date/time, size, drive and folder · instant search · sortable columns
- Review leftovers (folders, files, registry keys) and pick what to delete
- Debloat: telemetry, Start suggestions, Bing/Cortana, Copilot, Edge background/Startup Boost, animations, transparency, optional Edge removal
- Skips protected Windows SystemApps
- Live terminal showing every command and its output
- Dark / light theme · English / Português (BR)

## Build
Windows with .NET 8 SDK and WiX v4+:
```powershell
pwsh build.ps1
```
Outputs `dist\BareWin-<version>.exe` and `dist\BareWin-<version>-x64.msi`.

> Unsigned build: Windows SmartScreen will warn on first run.
