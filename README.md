# GitVulnGuard

## AI-Powered Vulnerability Detection in Git Commits

GitVulnGuard is a revolutionary tool that analyzes Git diffs in real-time using advanced AI models to detect potential security vulnerabilities, data leaks, and code quality issues before they reach production.

### Key Features

- **Real-time AI Analysis**: Leverages multiple specialized LLMs to analyze code changes during git operations
- **Vulnerability Prevention**: Detects security issues, hardcoded credentials, and infrastructure misconfigurations
- **Smart Diff Context**: Understands the full context of code changes across multiple files
- **Custom Policy Engine**: Define organization-specific security and quality policies
- **Integration with Modern AI Models**: Uses latest foundation models with code understanding capabilities

### Installation

```bash
pip install gitvulnguard
```

### Usage

```bash
# Install as a git hook
gitvulnguard install

# Manual scan
gitvulnguard scan --diff HEAD~1
```

### Configuration

Create a `gitvulnguard.yaml` in your project root:

```yaml
models:
  - name: security-llm
    endpoint: your-endpoint
policies:
  - no-hardcoded-secrets
  - secure-api-usage
```

### Requirements

- Python 3.10+
- Git 2.35+

### License

MIT
