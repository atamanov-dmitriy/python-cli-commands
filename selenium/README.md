## Создание проекта на Selenium

0) Установить [python](https://www.python.org/downloads/)
1) Создайте папку с проектом (название папки любое, например Selenium)
2) Внутри папки создайте два файла:
    - main.py
       ```
      from fastapi import FastAPI
      
      app = FastAPI()
      
      @app.get("/")
      def read_root():
          return {"message": "Привет, FastAPI!"}
      ```
    - requirements.txt
      ```
      fastapi[standard]
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
9) Для запуска проекта нужно ввести `fastapi dev main.py` или `uvicorn main:app --reload`
10) После успешного запуска перейти по ссылке `127.0.0.1:8000` или `localhost:8000`
