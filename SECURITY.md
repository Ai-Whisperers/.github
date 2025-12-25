# Security Policy

## Supported Versions

Please refer to each repository's README or releases page for supported versions.

## Reporting a Vulnerability

If you discover a security vulnerability in any Ai-Whisperers project, please report it responsibly:

### How to Report

Please use GitHub's **Private Vulnerability Reporting** feature. This allows you to open a secure, private issue that only repository maintainers can see.

1. Navigate to the **Security** tab of the repository.
2. Click the **Report a vulnerability** button.
3. In your report, please include:
   - Description of the vulnerability
   - Steps to reproduce
   - Potential impact
   - Suggested fix (if any)

We strictly prefer this method over email. If absolutely necessary, you may contact us at **support@aiwhisperers.com**.

### What to Expect

- **Acknowledgment**: Within 48 hours
- **Initial Assessment**: Within 7 days
- **Resolution Timeline**: Depends on severity
  - Critical: 7 days
  - High: 14 days
  - Medium: 30 days
  - Low: 60 days

### Disclosure Policy

- We follow coordinated disclosure
- Security fixes are prioritized
- Credit given to reporters (unless anonymity preferred)

## Security Best Practices

### Dependencies

We regularly scan for vulnerabilities:

```bash
pip-audit
bandit -r src/
```

### Safe Usage

- Run in sandboxed environments when processing untrusted data
- Do not pickle/unpickle model weights from untrusted sources
- Validate inputs before processing

### Data Handling

- Ensure compliance with relevant data protection regulations
- No personal health information (PHI) should be processed without proper safeguards

## Acknowledgments

We thank all security researchers who responsibly disclose vulnerabilities.
