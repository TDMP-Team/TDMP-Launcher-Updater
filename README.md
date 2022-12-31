# TDMP-Launcher-Updater
The top-level client application that handles auto-updating and launching the TDMP Launcher (which itself auto-updates TDMP and launches Teardown).

## Building self-contained package (with neccesary runtimes)
```
cd src\LauncherUpdater
dotnet publish -r win10-x64 --self-contained -c Release
```
Result will end up in `src\LauncherUpdater\bin\Release\net7.0-windows\win10-x64`  
A vast majority of the result files may not be neccesary, since the entire runtime and every dll it offers is bundled in with it.