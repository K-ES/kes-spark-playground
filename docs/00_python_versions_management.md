## Проверка установленных версий Python

Перед тем как наводить порядок, нужно понять, какие версии Python реально доступны в системе.

### PowerShell

Выполни команду:
```powershell
Get-Command python* |
Select-Object Name, Source |
Sort-Object Source