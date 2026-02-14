# Contributing to AI Whisperers

Thank you for your interest in contributing to our projects! We welcome contributions from developers, researchers, designers, and domain experts.

## 📋 Table of Contents
- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Code Standards](#code-standards)
- [Pull Request Process](#pull-request-process)
- [Types of Contributions](#types-of-contributions)
- [Project-Specific Guidelines](#project-specific-guidelines)
- [Community](#community)

## 📜 Code of Conduct

Please read and follow our [Code of Conduct](CODE_OF_CONDUCT.md). We are committed to providing a welcoming and inclusive environment for all contributors.

## 🚀 Getting Started

### Prerequisites
- **Git** for version control
- **GitHub account** for collaboration
- Project-specific requirements (check individual READMEs)

### First-Time Setup
1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/repository-name.git
   cd repository-name
   ```
3. **Add upstream remote**:
   ```bash
   git remote add upstream https://github.com/Ai-Whisperers/repository-name.git
   ```
4. **Create a branch** for your work:
   ```bash
   git checkout -b feature/your-feature-name
   ```

### Development Environment
Each project has specific setup instructions. Common patterns:

#### **TypeScript/Next.js Projects (Vete, etc.)**
```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Run tests
npm test

# Type checking
npm run typecheck

# Linting
npm run lint
```

#### **Python Projects (Research, AI)**
```bash
# Create virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
# venv\Scripts\activate   # Windows

# Install dependencies
pip install -r requirements.txt
pip install -r requirements-dev.txt  # if available

# Run tests
pytest

# Code quality
black . --check
isort . --check
ruff check .
```

## 🔄 Development Workflow

### Branch Strategy
- `main` - Production-ready code
- `develop` - Integration branch (if used)
- `feature/*` - New features
- `fix/*` - Bug fixes
- `docs/*` - Documentation updates
- `chore/*` - Maintenance tasks

### Commit Messages
Use [Conventional Commits](https://www.conventionalcommits.org/):
```
type(scope): description

[optional body]

[optional footer]
```

**Types:**
- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation
- `style:` - Formatting, missing semi-colons, etc.
- `refactor:` - Code restructuring
- `test:` - Adding or updating tests
- `chore:` - Maintenance, dependencies, tooling

**Examples:**
```
feat(auth): add Google OAuth integration
fix(api): resolve CORS issue with upload endpoint
docs(readme): update installation instructions
```

## 🎨 Code Standards

### General Principles
1. **Readability over cleverness** - Write code for humans first
2. **Consistency** - Follow existing patterns in the codebase
3. **Documentation** - Comment why, not what
4. **Testing** - Write tests for new functionality
5. **Security** - Never commit secrets, validate inputs

### TypeScript/JavaScript
- Use **TypeScript** for all new code
- **ESLint** with strict rules
- **Prettier** for formatting
- **No `any` types** - use proper typing
- **Functional components** with hooks
- **Error boundaries** for React apps

### Python
- **Black** for formatting (line length 120)
- **isort** for import sorting
- **ruff** for linting
- **mypy** for type checking
- **PEP 8** compliance
- **Type hints** for all new code

### Documentation
- **README.md** - Project overview and quick start
- **API documentation** - For libraries and APIs
- **Inline comments** - Explain complex logic
- **Docstrings** - For all public functions/classes
- **Architecture decisions** - Record in ADRs

## 🔧 Pull Request Process

### Before Submitting
1. **Sync with upstream**:
   ```bash
   git fetch upstream
   git rebase upstream/main
   ```
2. **Run tests** - Ensure all tests pass
3. **Check code quality** - Run linters and formatters
4. **Update documentation** - Keep docs in sync with changes
5. **Squash commits** - One logical change per commit

### PR Checklist
- [ ] Title follows conventional commit format
- [ ] Description explains what and why, not just how
- [ ] Tests added/updated for new functionality
- [ ] Documentation updated
- [ ] Code follows project standards
- [ ] No breaking changes (or clearly documented)
- [ ] Linked to relevant issues

### Review Process
1. **Automated checks** - CI/CD pipelines run
2. **Code review** - At least one maintainer approval required
3. **Address feedback** - Respond to review comments
4. **Merge** - Squash and merge when approved

## 🎯 Types of Contributions

### Code Contributions
- Bug fixes
- New features
- Performance improvements
- Refactoring
- Test coverage

### Documentation
- Tutorials and guides
- API documentation
- Translation/localization
- Code examples
- Architecture documentation

### Design & UX
- UI/UX improvements
- Accessibility enhancements
- Design system components
- User research

### Research & Analysis
- Algorithm improvements
- Benchmark results
- Data analysis
- Academic contributions

### Community Support
- Answering questions
- Triaging issues
- Mentoring new contributors
- Writing blog posts

## 📁 Project-Specific Guidelines

### Vete (Veterinary Platform)
- **Priority:** Production stability and security
- **Testing:** 100% test coverage for critical paths
- **Security:** GDPR compliance, data protection
- **UI/UX:** Mobile-first, Spanish language focus

### Research Projects
- **Reproducibility:** Include environment specs
- **Documentation:** Methodology and results
- **Data:** Follow ethical guidelines
- **Publication:** Coordinate with research team

### Infrastructure & Tools
- **Reliability:** High availability requirements
- **Monitoring:** Include observability
- **Documentation:** Deployment and operations
- **Security:** Least privilege principle

## 👥 Community

### Communication
- **GitHub Issues** - For bugs and feature requests
- **GitHub Discussions** - For questions and ideas
- **Pull Requests** - For code contributions
- **Email** - For sensitive or private matters

### Getting Help
1. Check existing documentation
2. Search issues and discussions
3. Ask in GitHub Discussions
4. Contact maintainers if urgent

### Recognition
Contributors are recognized through:
- GitHub contributor graph
- Release notes
- Project documentation
- Team acknowledgments

## 📝 License

By contributing, you agree that your contributions will be licensed under the same license as the project. Most projects use:
- **PolyForm Noncommercial License** - For research and tools
- **Proprietary licenses** - For commercial products
- **MIT/Apache 2.0** - For open-source utilities

Check individual repository LICENSE files for specifics.

## 🙏 Thank You!

Your contributions help us build better tools and advance AI research. We appreciate your time and effort!

---

*This document is maintained by the AI Whisperers team. Last updated: February 2026*