# Додавання тексту на початок назв файлів за допомогою PowerShell

Цей інструктаж допоможе вам додати текст на початок назв усіх файлів у папці за допомогою PowerShell.

## Кроки

1. Відкрийте **PowerShell**:
   - Натисніть `Win + S` та введіть **PowerShell**.
   - Запустіть PowerShell.

2. Перейдіть до потрібної папки:
   ```powershell
   cd "C:\Users\Ім'я\Documents\МояПапка"

3. Виконайте команду для зміни назв файлів:
   ```powershell
   Get-ChildItem -File | Rename-Item -NewName { "ім'я_" + $_.Name }
