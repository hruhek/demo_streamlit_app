# Demo Streamlit App

A minimal Python application template designed for Streamlit integration and rapid prototyping.

## Overview

This project provides a clean starting point for building Streamlit applications with modern Python tooling. Currently contains a basic "Hello World" application that can be easily extended with Streamlit components.

## Quick Start

### Prerequisites

- Python 3.13 or higher
- [uv](https://github.com/astral-sh/uv) package manager

### Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd demo_streamlit_app
   ```

2. Install dependencies:

   ```bash
   uv sync
   ```

## Development

### Adding Dependencies

Use `uv` to manage dependencies:

```bash
# Add a new package
uv add package-name

# Add development dependencies
uv add --dev pytest

# Install all dependencies
uv sync
```

## Running the App

```bash
# With Streamlit (after adding streamlit dependency)
uv run streamlit run main.py
```
