2026.01.10 05:20 Тестовая запись  
**2026.01.10 05:20 Тестовая запись 22222222222222222222222222222222222222222222222222222222222222222222222222222222222222**

## 2026.01.10 05:20

### 7. OSS contribution (first PR)
- Впервые сделал **Pull Request в чужой репозиторий**
- Пройден полный OSS-флоу:
  - fork → локальная ветка → коммиты → push → PR
- Исправлены неточности в README без изменения логики проекта
- Добавлены platform-specific инструкции (Windows PowerShell)
- Git identity настроен локально для репозитория
- PR отправлен и опубликован — зафиксирован публичный след в истории GitHub

**Итог:**  
Первый осознанный PR в чужой проект выполнен корректно и по стандартному OSS-процессу.


### 7. OSS contribution (first PR)
- Submitted my **first Pull Request to a third-party repository**
- Completed the full OSS workflow:
  - fork → feature branch → commits → push → PR
- Fixed documentation inaccuracies without changing project logic
- Added platform-specific instructions (Windows PowerShell)
- Git identity configured locally for this repository
- PR published, leaving a public contribution trace on GitHub

**Result:**  
First intentional OSS Pull Request completed correctly using the standard open-source workflow.


## 2026.01.09 11:54

**Date:** 2026-01-09  
**Project:** kes-spark-playground  
**OS:** Windows  
**IDE:** PyCharm  
**Mode:** local Spark + Jupyter

---

### 1. Python & venv
- Создано виртуальное окружение `.venv`
- PyCharm не активировал venv автоматически:
  - причина: venv был создан **после** открытия проекта
- Решение:
  - выбрать `.venv` как **Python Interpreter проекта**
  - перезапустить терминал / kernel

---

### 2. Jupyter & kernel
- PyCharm открывает `.ipynb` через **IDE-managed Jupyter**
- По умолчанию kernel = **system Python**
- Активированный venv в терминале **не влияет** на Jupyter
- Решение:
  - привязка kernel к интерпретатору проекта
  - PyCharm автоматически установил `ipykernel` при первом запуске ячейки
- Проверка:
  ```python
  import sys
  sys.executable


## 2026.01.08 03:05
Тест

**RU:**  
Spark. Старт изучения.

**EN:**  
Spark. Start of learning. 
