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