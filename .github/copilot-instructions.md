# Copilot Instructions for demo-streamlit-app

## Project Overview
- This is a minimal Python application template designed for Streamlit integration and rapid prototyping.
- The main entry point is `main.py`, which currently prints a greeting. No Streamlit code is present yet, but the project is structured for easy extension.
- Project metadata and dependencies are managed via `pyproject.toml`. No external dependencies are currently specified.
- Uses `uv` for fast Python package management and virtual environment handling.

## Key Files
- `main.py`: Application entry point. Extend this file for app logic.
- `pyproject.toml`: Project configuration, Python version (>=3.13), dependencies.
- `README.md`: Comprehensive documentation with setup, development workflows, and Streamlit integration guide.

## Developer Workflows
- **Setup project:**
  ```bash
  uv sync  # Install dependencies and create virtual environment
  ```
- **Add dependencies:**
  ```bash
  uv add <package-name>          # Regular dependency
  uv add --dev <package-name>    # Development dependency
  ```
- **Run the basic app:**
  ```bash
  uv run main.py
  ```
- **Run as Streamlit app (after adding streamlit):**
  ```bash
  uv run streamlit run main.py
  ```
- **Testing:**
  - No test framework or test files are present. Add tests in a `tests/` directory and update instructions here if testing is added.

## Conventions & Patterns
- **Dependency Management:** Uses `uv` for fast Python package management. Always use `uv add` instead of `pip install`.
- Minimal structure; follow standard Python conventions.
- Extend `main.py` for new features. If adding Streamlit, import and use `streamlit` in this file or in new modules.
- Keep project metadata up to date in `pyproject.toml`.

## Integration Points
- No external services or APIs are integrated yet.
- If adding Streamlit, document usage and UI patterns here.

## Example Extension
To add a basic Streamlit UI:
```python
import streamlit as st

def main():
    st.title("Demo Streamlit App")
    st.write("Hello from Streamlit!")

if __name__ == "__main__":
    main()
```

## Guidance for AI Agents
- Prefer updating `main.py` for new features unless a larger structure is needed.
- Document new workflows and conventions in this file as the project grows.
- Keep instructions concise and project-specific.
