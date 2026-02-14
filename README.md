# Steps for new projects

Description: Sample pyproject.toml and scalfold for new projects

0. Scaffold recommended

        myapp/
        ├── pyproject.toml
        ├── README.md
        ├── .gitignore
        ├── docs/
        ├── src/
        │   └── myapp/
        │       ├── __init__.py
        │       └── main.py
        └── tests/
            └── test_main.py
    

1. Init with UV, just choose one.
    
        uv init . --no-readme
        uv init . --bare
        uv init myapp & cd myapp

2. Venv

        uv venv

3. Add yours dependencies

        uv add requests
        uv add --dev pytest ruff mypy

4. Execute with no venv 

        uv run myapp

5. Lint

        uv run ruff check .


