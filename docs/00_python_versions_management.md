## Проверка установленных версий Python

Перед тем как наводить порядок, нужно понять, какие версии Python реально доступны в системе.

### PowerShell

Выполни команду:
```powershell
Get-Command python* |
Select-Object Name, Source |
Sort-Object Source
```

Получишь примерно следующее:
```text
Name               Source
----               ------
python.exe         C:\Python\Python312\python.exe
python_d.exe       C:\Python\Python312\python_d.exe
pythonw.exe        C:\Python\Python312\pythonw.exe
pythonw_d.exe      C:\Python\Python312\pythonw_d.exe
python.exe         C:\Python32bit\python.exe
python_d.exe       C:\Python32bit\python_d.exe
python3.13t.exe    C:\Python32bit\python3.13t.exe
python3.13t_d.exe  C:\Python32bit\python3.13t_d.exe
pythonw.exe        C:\Python32bit\pythonw.exe
pythonw_d.exe      C:\Python32bit\pythonw_d.exe
pythonw3.13t.exe   C:\Python32bit\pythonw3.13t.exe
pythonw3.13t_d.exe C:\Python32bit\pythonw3.13t_d.exe
python.exe         C:\Python64bit\python.exe
pythonw.exe        C:\Python64bit\pythonw.exe
python.exe         C:\Users\ekriv\AppData\Local\Microsoft\WindowsApps\python.exe
python3.exe        C:\Users\ekriv\AppData\Local\Microsoft\WindowsApps\python3.exe
```