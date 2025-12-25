# Contributing to Ai-Whisperers Projects

Thank you for your interest in contributing! Our projects welcome contributions from researchers, students, and the open-source community.

## License Agreement

By contributing to our projects, you agree that your contributions will be licensed under the project's existing license (typically **PolyForm Noncommercial License 1.0.0**). This means:

- Your contributions remain free for academic and research use
- Commercial entities cannot use your contributions without a separate license
- You retain copyright to your contributions

## Getting Started

### Prerequisites

- Python 3.8+ (3.10+ recommended)
- See individual project READMEs for specific requirements

### Development Setup

```bash
# Clone the repository
git clone https://github.com/Ai-Whisperers/<repository-name>.git
cd <repository-name>

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Install development dependencies
pip install pytest black isort flake8 mypy ruff

# Run tests to verify setup
pytest
```

## Code Style

We follow these conventions:

- **Formatter**: `black` (line length 120)
- **Import sorting**: `isort`
- **Linting**: `ruff` and `flake8`
- **Type checking**: `mypy`

### Before Submitting

```bash
# Format code
black src/ tests/ --line-length 120
isort src/ tests/

# Run linting
ruff check src/
flake8 src/

# Run type checking
mypy src/

# Run tests
pytest
```

## Types of Contributions

### Bug Reports

Open an issue with:
- Clear description of the bug
- Steps to reproduce
- Expected vs actual behavior
- System information (Python version, relevant library versions)

### Feature Requests

Open an issue describing:
- The problem you're trying to solve
- Your proposed solution
- Alternative approaches considered

### Code Contributions

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Make your changes
4. Add tests for new functionality
5. Ensure all tests pass
6. Submit a pull request

### Documentation

- Fix typos or unclear explanations
- Add examples
- Improve docstrings
- Write tutorials

### Research Contributions

- Share experimental results
- Propose new architectures or methodologies
- Contribute datasets
- Write analysis notebooks

## Pull Request Process

1. **Title**: Use conventional commit format
   - `feat: Add new feature`
   - `fix: Correct bug`
   - `docs: Update documentation`
   - `test: Add tests`

2. **Description**: Explain what and why, not just how

3. **Tests**: Include tests for new features

4. **Documentation**: Update relevant docs

5. **Review**: Address reviewer feedback promptly

## Questions?

- Open a GitHub issue for technical questions
- Email support@aiwhisperers.com for licensing questions
- Check existing issues and documentation first

## Recognition

Contributors will be acknowledged in:
- AUTHORS.md
- Release notes
- Academic publications (where appropriate)

Thank you for contributing to open science!
