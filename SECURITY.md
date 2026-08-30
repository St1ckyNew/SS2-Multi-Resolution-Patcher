# Security

If you believe the patcher has a security issue, avoid posting sensitive information in a public issue.

For ordinary crashes, game compatibility problems, false-positive antivirus reports, or graphical problems, use the GitHub issue tracker.

## Release verification

Official releases should include a SHA-256 checksum for `SS2MultiResPatcher.exe`.

On Windows PowerShell:

```powershell
Get-FileHash .\SS2MultiResPatcher.exe -Algorithm SHA256
```

Compare the result with the checksum shown on the GitHub Release page.

Do not trust binaries from third-party mirrors if they do not match the official checksum.
