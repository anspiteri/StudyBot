# Study
A personal study tool that automates tasks that I do regularly.

I wanted to use the opportunity presented in wanting to learn tooling & AI integration to create something that I could use. The goal with this tool is to able to automate a few tasks that I do regularly with LLMs for university, namely note summarisation and anki / flash card generation.

## Structure
```
study-automation-tool/
├── pyproject.toml
├── README.md
├── LICENSE
└── src/
    └── study_tool/
        ├── __init__.py
        ├── cli.py
        ├── config.py
        └── core/
            ├── __init__.py
            ├── pdf_parser.py
            ├── summariser.py
            └── card_generator.py
```

# Development
1. Setup virtual environment for environment isolation: `python -m venv .venv`
2. Activate virtual environment: `source .venv/bin/activate` (Linux)
3. Install project executable & dependencies: `pip install -e .` ('e' - for editable, sources from `src` files.)

## Usage
In command line type: `study`

## Future Build Options
1. `pip install .` - copies project to `.venv` site packages
2. `python -m build` - builds a "wheel"
3. Create a binary using `pyinstaller`, `pex`, or `shiv`
