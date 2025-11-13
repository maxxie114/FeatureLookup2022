# Contributing to FeatureLookup2022

Thank you for your interest in contributing to FeatureLookup2022! This document provides guidelines and instructions for contributing.

## Code of Conduct

This project aims to foster an inclusive and respectful environment. Please be kind and courteous in all interactions.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include:

- **Clear title and description**
- **Steps to reproduce** the behavior
- **Expected behavior** vs. actual behavior
- **Python version** and operating system
- **Any error messages** or logs

Example:
```
Title: Program crashes when using compare with invalid phoneme

Steps to reproduce:
1. Start the program
2. Type: compare x y z
3. Press Enter

Expected: Error message about invalid phonemes
Actual: Program crashes with TypeError

Environment:
- Python 3.12
- Ubuntu 22.04
```

### Suggesting Features

Feature suggestions are welcome! Please include:

- **Clear description** of the feature
- **Use case**: Why is this feature needed?
- **Example usage**: How would users interact with it?
- **Potential implementation ideas** (if you have any)

### Pull Requests

1. **Fork the repository** and create your branch from `main`
2. **Make your changes**:
   - Follow the existing code style
   - Add comments for complex logic
   - Update documentation if needed
3. **Test your changes**:
   - Run the program and test affected commands
   - Test edge cases
   - Ensure no existing functionality is broken
4. **Commit your changes**:
   - Use clear, descriptive commit messages
   - Reference issues if applicable (e.g., "Fixes #123")
5. **Push to your fork** and submit a pull request

## Development Guidelines

### Code Style

- Follow PEP 8 guidelines for Python code
- Use meaningful variable and function names
- Add docstrings for functions
- Keep functions focused and modular

### Testing

Before submitting:
- Test all modified commands
- Test with various phonemes and features
- Test edge cases (empty input, invalid phonemes, etc.)
- Ensure the program starts and exits cleanly

### Documentation

- Update README.md if you add features or change usage
- Add inline comments for complex logic
- Update help text if you modify commands

## Project Structure

```
FeatureLookup2022/
├── FeatureLookup2022.py    # Main program file
├── README.md               # Project documentation
├── LICENSE                 # License file
└── CONTRIBUTING.md         # This file
```

## Feature Requests and Ideas

Here are some ideas for contributions:

### Easy
- Add more abbreviations for features
- Improve error messages
- Add color coding to output
- Add command history support

### Medium
- Add support for phoneme diacritics
- Implement export to CSV/JSON
- Add batch processing from file
- Create a simple GUI

### Advanced
- Add natural class detection
- Implement phonological rules
- Add feature geometry visualization
- Create a web-based interface

## Questions?

Feel free to open an issue with the "question" label if you need help or clarification.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.

Thank you for contributing to FeatureLookup2022! 🎉
