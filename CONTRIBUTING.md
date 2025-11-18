# Contributing to Cloud Security Scanner

First off, thank you for considering contributing to Cloud Security Scanner! It's people like you that make this tool better for everyone.

## Code of Conduct

This project and everyone participating in it is governed by our Code of Conduct. By participating, you are expected to uphold this code.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check the existing issues to avoid duplicates. When you create a bug report, include as many details as possible:

- **Use a clear and descriptive title**
- **Describe the exact steps to reproduce the problem**
- **Provide specific examples**
- **Describe the behavior you observed and what you expected**
- **Include screenshots if relevant**
- **Include your environment details** (OS, Node version, etc.)

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion:

- **Use a clear and descriptive title**
- **Provide a detailed description of the suggested enhancement**
- **Explain why this enhancement would be useful**
- **List some examples of how it would be used**

### Pull Requests

1. **Fork the repository** and create your branch from `main`
2. **Make your changes** and test thoroughly
3. **Follow the coding style** of the project
4. **Write clear commit messages**
5. **Include tests** if applicable
6. **Update documentation** as needed
7. **Submit a pull request**

## Development Setup

1. Clone your fork:
```bash
git clone https://github.com/YOUR_USERNAME/cloud-security-scanner.git
cd cloud-security-scanner
```

2. Install dependencies:
```bash
npm install
```

3. Create a branch:
```bash
git checkout -b feature/my-feature
```

4. Make your changes and test:
```bash
npm run dev
```

5. Commit your changes:
```bash
git add .
git commit -m "Add my feature"
```

6. Push to your fork:
```bash
git push origin feature/my-feature
```

7. Open a Pull Request

## Coding Guidelines

### JavaScript/React

- Use ES6+ features
- Follow React best practices and hooks guidelines
- Use functional components over class components
- Keep components small and focused
- Use meaningful variable and function names

### Backend

- Follow RESTful API design principles
- Implement proper error handling
- Add logging for important operations
- Validate all inputs
- Handle edge cases

### Git Commit Messages

- Use present tense ("Add feature" not "Added feature")
- Use imperative mood ("Move cursor to..." not "Moves cursor to...")
- Limit the first line to 72 characters
- Reference issues and pull requests after the first line

Examples:
```
Add AWS Lambda vulnerability scanning
Fix credential validation bug
Update documentation for Azure setup
```

## Testing

Before submitting:

1. Test your changes locally
2. Ensure all existing tests pass
3. Add new tests for new features
4. Test with different cloud providers if applicable

## Documentation

- Update README.md if you change functionality
- Add JSDoc comments for new functions
- Update API documentation if you change endpoints
- Include examples for new features

## Security

- **Never commit credentials or secrets**
- Follow secure coding practices
- Report security vulnerabilities privately to the maintainers
- Use encryption for sensitive data

## Questions?

Feel free to open an issue with the tag `question` if you need help or clarification.

## Recognition

Contributors will be recognized in our README.md file.

Thank you for contributing! 🎉
