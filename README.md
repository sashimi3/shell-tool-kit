# shell-tool-kit

Shell tool kit

## Security Risks of Using curl and bash Combination for Script Execution

Using the combination of the curl and bash commands to execute scripts is not recommended due to security risks. Here's why:

- Trustworthiness Concerns: It's difficult to ensure that the source of the script is trustworthy. A script downloaded via the curl command might contain unexpected malicious code.
- Security Vulnerabilities: Executing a script with the bash command sourced from an untrusted origin can introduce significant security vulnerabilities to the system. Malicious scripts may execute code intended to harm the user's system.
- Management Complexity: Managing and troubleshooting scripts executed using the curl and bash combination can be challenging. Version control, updates, and dependency management of external scripts become difficult.

Instead, it's recommended to review the source of the script before downloading and executing it. If possible, download scripts from trusted sources and execute them locally.

## Usage

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/sashimi3/shell-tool-kit/main/init_wsl_python.sh)"
```
