# Troubleshooting

## The game is not detected

Use **Browse** and select:

```text
...\Sudden Strike 2 Gold\code\Release
```

or the main game directory:

```text
...\Sudden Strike 2 Gold
```

The selected location must ultimately contain:

```text
n2Cad1024.dll
n2Game_Dll.dll
```

## The patcher says the DLL pair is unknown

The game files may already have been modified by another patch, mod, or previous manual edit.

Recommended recovery:

1. Use **Restore Backup** if a valid patcher backup exists.
2. Otherwise use Steam:
   **Properties → Installed Files → Verify integrity of game files**.
3. Start the patcher again.

Do not force-patch an unknown installation unless you know why the files differ.

## Windows SmartScreen appears

The patcher is an unsigned community executable. SmartScreen can warn about newly released binaries that do not yet have reputation.

Only download from the official GitHub release page and compare the executable's SHA-256 checksum with the checksum published in the release notes.

## Access denied / patch cannot be installed

Steam is commonly installed inside `Program Files (x86)`, which is protected by Windows.

The application includes an administrator manifest. Accept the UAC prompt when starting it.

Also make sure the game is not currently running.

## Game does not start after patching

1. Close the game.
2. Use **Restore Backup**.
3. Test the original state.
4. If necessary, verify the game files through Steam.
5. Open a GitHub issue with the patcher log.

## Graphical problem at a custom resolution

Include all of the following in the bug report:

- exact width and height
- screenshot
- map / mission if relevant
- whether 1920×1080 works correctly on the same installation
- patcher log
- DLL state shown before patching

## Resolution is rejected

The current public release is intentionally limited to a maximum of:

```text
1920 × 1080
```

The width must be even.

Higher resolutions require additional engine work and are not enabled by the current release.
