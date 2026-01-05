# Contributing to Breast Cancer Detection

Thank you for your interest in contributing to this project! This document provides guidelines and steps for contributing.

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Pull Request Process](#pull-request-process)
- [Style Guidelines](#style-guidelines)

## Code of Conduct

This project adheres to a code of conduct. By participating, you are expected to uphold this code. Please be respectful and constructive in all interactions.

## How Can I Contribute?

### 🐛 Reporting Bugs

- Check if the bug has already been reported in Issues
- Use the bug report template
- Include detailed steps to reproduce
- Add screenshots if applicable

### 💡 Suggesting Enhancements

- Open an issue with the enhancement label
- Clearly describe the feature and its benefits
- Provide examples of how it would work

### 🔧 Code Contributions

1. **Bug fixes**: Fix existing issues
2. **New features**: Add new ML models or visualizations
3. **Documentation**: Improve README or add docstrings
4. **Tests**: Add unit tests

## Development Setup

1. Fork and clone the repository

   ```bash
   git clone https://github.com/yourusername/breast-cancer-detection.git
   cd breast-cancer-detection
   ```

2. Create a virtual environment

   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   ```

3. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

## Pull Request Process

1. Create a feature branch

   ```bash
   git checkout -b feature/your-feature-name
   ```

2. Make your changes and commit

   ```bash
   git commit -m "Add: description of your changes"
   ```

3. Push to your fork

   ```bash
   git push origin feature/your-feature-name
   ```

4. Open a Pull Request with:
   - Clear description of changes
   - Reference to related issues
   - Screenshots (if UI changes)

## Style Guidelines

### Python Code Style

- Follow PEP 8 guidelines
- Use meaningful variable names
- Add docstrings to functions
- Keep functions focused and small

### Commit Messages

Use conventional commits:

- `Add:` for new features
- `Fix:` for bug fixes
- `Docs:` for documentation
- `Refactor:` for code refactoring

## Questions?

Feel free to open an issue for any questions!
