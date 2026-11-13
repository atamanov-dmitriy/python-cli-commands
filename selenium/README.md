## Создание проекта на Selenium

0) Установить [python](https://www.python.org/downloads/)
1) Создайте папку с проектом (название папки любое, например Selenium)
2) Внутри папки создайте два файла:
    - main.py (пустой)
    - requirements.txt
      ```
      selenium==4.*
      ```

4) Откройте папку в VSCode
5) Откройте терминал VSCode через `Ctrl + Ё` или другой терминал (например git bash или PowerShell)
6) Введите команду в терминале `python -m venv venv` для создания виртуального окружения
   Критерий выполнения: Должна создаться папка `venv`
7) Активация venv
    - `.\venv\Scripts\Activate.ps1` - активировать окружение в PowerShell
    - `venv/Scripts/activate` - активировать окружение в Bash
    Критерий выполнения: В терминале должно появиться `(venv)`
8) `pip install -r requirements.txt`
9) Для запуска скрипта нужно ввести `python main.py`
