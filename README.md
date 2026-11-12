# Project Cars for RE_Kenshi

Project Cars adds modular drivable vehicles to Kenshi. The native plugin runs under
[RE_Kenshi](https://github.com/BFrizzleFoShizzle/RE_Kenshi) and links against
[KenshiLib](https://github.com/BFrizzleFoShizzle/KenshiLib).

## Extra-small vehicles in 0.8.19

Research **Vehicle Mechanics I**, then **Extra-Small Frames** to unlock the
four-wheel quad and two-wheel motorcycle. Both have fitted spawn presets in
**Ctrl+F12 → Spawn Vehicle**. Version 0.8.19 raises road speeds and improves
throttle response in manual and route driving.

## Build

Use Visual C++ 2010 x64, Windows SDK 7.1, and the
[KenshiLib example dependencies](https://github.com/BFrizzleFoShizzle/KenshiLib_Examples_deps).
The build script lists the expected toolchain layout. Pass the parent directory
that contains `toolchain` and `KenshiLib_Examples_deps`.

```powershell
.\tools\build.ps1 -KenshiProjects 'C:\path\to\dependencies'
```

The script emits a Release x64 DLL and PDB under `build/`. Running the plugin
requires a compatible RE_Kenshi installation and matching Project Cars game data
and assets.

## License

Project Cars source is licensed under [GNU GPL version 3 only](LICENSE).
The adapted KenshiLib header retains its upstream provenance in
[plugin/compat/README.md](plugin/compat/README.md). External dependencies retain
their respective licenses.
