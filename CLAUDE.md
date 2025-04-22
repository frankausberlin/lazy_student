# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands
- `pip install -e .` - Install in development mode
- `nbdev_prepare` - Compile changes from notebooks to Python
- `nbdev_preview` - Preview documentation
- `nbdev_export` - Export code from notebooks to Python
- `nbdev_install_hooks` - Install Git hooks

## Code Style Guidelines
- Code is written in Jupyter notebooks (nbs/*.ipynb) and automatically exported to Python
- Follow standard Python naming conventions with snake_case for functions and variables
- Comment key functionality using markdown cells in notebooks
- One function/class per notebook cell with clear markdown documentation
- No explicit type annotations required
- Error handling should follow Python idioms (try/except where appropriate)
- Keep imports organized by standard library, then third-party packages, then local modules
- No specific test framework - tests are written in notebook cells

## Notes
- nbdev project: code in notebooks, Python modules auto-generated - don't edit directly
- Documentation is auto-generated from notebooks
- Make all code changes in notebooks, then run nbdev_prepare to update Python modules