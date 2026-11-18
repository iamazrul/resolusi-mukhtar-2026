# Nota GitHub

## Ralat `detected dubious ownership`

Folder repo ini dicipta menggunakan akaun sandbox `CodexSandboxOffline`. Apabila Git dijalankan melalui akaun Windows sendiri, Git mungkin menyekat repo kerana pemilik folder berbeza.

Jalankan arahan berikut dalam PowerShell menggunakan akaun Windows sendiri untuk mempercayai repo ini sahaja:

```powershell
git config --global --add safe.directory "D:/Works/codes/github_flow/resolusi-mukhtar-2026"
```

Kemudian push perubahan ke GitHub:

```powershell
git -C "D:\Works\codes\github_flow\resolusi-mukhtar-2026" push origin main
```

Lengkapkan login GitHub jika diminta. Jangan kongsi kata laluan atau token dalam chat.

Push ke `main` akan mencetuskan workflow GitHub Actions untuk deploy laman ke GitHub Pages secara automatik. Semak status di:

https://github.com/iamazrul/resolusi-mukhtar-2026/actions

Arahan `safe.directory` hanya perlu dijalankan sekali bagi akaun Windows ini, selagi lokasi repo tidak berubah.
