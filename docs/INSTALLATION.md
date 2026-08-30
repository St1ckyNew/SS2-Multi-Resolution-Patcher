# Installation

## Steam installation

The current Steam version normally loads its runtime files from:

```text
C:\Program Files (x86)\Steam\steamapps\common\Sudden Strike 2 Gold\code\Release
```

The patcher searches Steam and additional Steam libraries automatically and prioritizes this runtime directory.

## Normal installation

1. Download `SS2MultiResPatcher.exe` from the GitHub Releases page.
2. Run it.
3. Allow administrator access if Windows requests it.
4. Confirm the **Patch target** shown by the GUI.
5. Select a preset or enter a custom resolution.
6. Click **Install Patch**.
7. Launch the game normally through Steam.

The patcher modifies:

```text
n2Cad1024.dll
n2Game_Dll.dll
```

Other files in `code\Release` are not modified by the current resolution patch.

## Manual path selection

If auto detection does not find your installation, click **Browse**.

You can select either:

### The actual DLL folder

For example:

```text
...\Sudden Strike 2 Gold\code\Release
```

If the required DLLs are present directly in the selected folder, that exact folder is used.

### The main game folder

For example:

```text
...\Sudden Strike 2 Gold
```

If the required DLLs are not directly in that folder, the patcher automatically checks:

```text
code\Release
```

## Generate without installing

Use **Generate Files...** if you want the patcher to create the modified DLL pair in a separate directory without replacing your active game files.

## Backup

The first install creates:

```text
SS2_MultiRes_Backup
```

The backup is stored next to the DLLs being patched.

Do not delete this directory if you want to use the GUI's one-click restore function.
