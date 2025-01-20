# features

cd "C:\Users\Ім'я\Documents\МояПапка"
Get-ChildItem -File | Rename-Item -NewName { "ім'я_" + $_.Name }
