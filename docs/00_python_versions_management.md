## 01. Проверка установленных версий Python

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

Выполни команду:
```powershell
py -0p
```

Получишь примерно следующее:
```text
 -V:3.13t-32 *    C:\Python32bit\python3.13t.exe
 -V:3.13-32       C:\Python32bit\python.exe
 -V:3.12          C:\Python\Python312\python.exe
 -V:3.11          C:\Python64bit\python.exe
```

## 02. Полное удаление всех Python из системы (Windows)

⚠️ Делай это только если хочешь начать с чистого листа.

### 1. Удалить Python через «Приложения»
- Открой **Параметры → Приложения → Установленные приложения**
- Удали **все записи**, содержащие:
  - Python
  - Python Launcher
  - Python 3.x
- Отдельно проверь и удали:
  - **Python (Microsoft Store)**

---

### 2. Удалить Python из Microsoft Store
- Открой **Microsoft Store**
- Найди `Python`
- Удали все установленные версии

---

### 3. Удалить каталоги вручную
Проверь и удали, если существуют:

```text
C:\Python\
C:\Python32bit\
C:\Python64bit\
C:\Program Files\Python*
C:\Program Files (x86)\Python*
C:\Users\<user>\AppData\Local\Programs\Python\
