# AWS CDK Extension Pack

This is a collection of extensions that I've curated in this vscode extension pack to help you build, deploy and manage your AWS CDK applications.

<!-- TIP-LIST:START -->
> [!TIP]
> **We eliminate AWS complexity so you ship faster, spend less, and stay compliant.**
>
> Our managed AWS service gives you three things: a production-grade AWS CDK Landing Zone with built-in compliance controls, proactive monitoring that stops cost waste and security drift, and senior AWS expertise that speeds up your team's delivery.
>
> Book a free demo to see where you stand and what we'd fix first:
>
> <a href="https://towardsthecloud.com/services/aws-cdk-landing-zone#cta"><img alt="Book a Free Demo" src="https://img.shields.io/badge/Book%20a%20Free%20Demo-success.svg?style=for-the-badge"/></a>
>
> <details>
> <summary>⚡ <strong>See the symptoms of a missing AWS foundation and how we solve them</strong></summary>
> <br/>
>
> AWS starts simple. Then you scale: production and staging blur together, resources multiply without owners, IAM policies accumulate exceptions, security findings pile up in backlogs, and the bill climbs month after month.
>
> Those are symptoms of a missing AWS foundation. Without one, your developers spend more time fixing problems than shipping features.
>
> **We provide that foundation and own it entirely, so your team focuses on shipping, not firefighting.**
>
> ### Here's what's included:
>
> **1. We Provision a Secure [AWS CDK Landing Zone](https://towardsthecloud.com/services/aws-cdk-landing-zone) That Accelerates Compliance**
> - Multi-account architecture with security controls and compliance guardrails from day one
> - Scores 100% on the [CIS AWS Foundations Benchmark](https://docs.aws.amazon.com/securityhub/latest/userguide/cis-aws-foundations-benchmark.html) and 96% on [AWS Foundational Security Best Practices](https://docs.aws.amazon.com/securityhub/latest/userguide/fsbp-standard.html)
> - Those benchmarks map straight to **SOC 2**, **HIPAA**, and **PCI-DSS** controls, cutting months from your compliance timeline
>
> **2. We Monitor Proactively to Stop Cost Waste and Security Drift**
> - Quarterly cost reviews catch unattached volumes, oversized instances, and orphaned resources before they compound. AWS spend drops 20-30% on average, with [outliers hitting 60+%](https://towardsthecloud.com/services/aws-cost-optimization#case-study)
> - Continuous security monitoring across all accounts catches misconfigurations immediately. You get alerts while issues are still fixable, not after they're breaches
>
> **3. We Provide Senior AWS Expertise That Speeds Up Delivery**
> - Your developers get production-ready IaC templates for common patterns: multi-AZ applications, event-driven architectures, secure data pipelines. What takes weeks of research ships in hours
> - Architecture guidance on VPC design, IAM policies, disaster recovery, and observability from engineers who've solved these problems at enterprise scale
>
> [*"We achieved a perfect security score in days, not months."*](https://towardsthecloud.com/blog/case-study-accolade)
> *Galen Simmons, CEO of Accolade (Y Combinator startup)*
>
> </details>
<!-- TIP-LIST:END -->

## Included Extensions

This extension pack includes the following VS Code extensions:

1. **AWS Toolkit for Visual Studio Code**: Provides support for developing AWS applications
2. **Biome**: A performant linter, formatter, and more for JavaScript, TypeScript, and JSON
3. **Boto3 IDE**: Provides intelligent code completion, type checking, and documentation for AWS boto3 SDK
4. **Ruff**: An extremely fast Python linter and code formatter
5. **CDK Snippets**: Code snippets for AWS CDK development
6. **AWS IAM Actions Snippets**: Adds autocomplete and snippets for all AWS IAM policy actions
7. **AWS IAM Service Principal Snippets**: Autocompletion for AWS service principals.
8. **Draw.io Integration**: Integrates Draw.io diagrams into VS Code
9. **Docker**: Makes it easy to create, manage, and debug containerized applications
10. **Python**: IntelliSense, linting, debugging, and more for Python
11. **Pylance**: Fast, feature-rich language support for Python
12. **IntelliCode API Usage Examples**: AI-assisted code examples for API usage
13. **IntelliCode**: AI-assisted development features

## Installation

1. Open Visual Studio Code
2. Go to the Extensions view (Ctrl+Shift+X or Cmd+Shift+X on macOS)
3. Search for "AWS CDK Extension Pack"
4. Click "Install"

## Configuration

After installation, you can configure the extensions to suit your preferences. Here are some recommended settings to add to your `settings.json` file:

```json
{
  // Biome
  "[json][jsonc]": {
    "editor.defaultFormatter": "biomejs.biome",
    "editor.tabSize": 2
  },
  "[typescript][javascript]": {
    "editor.codeActionsOnSave": {
      "quickfix.biome": "explicit",
      "source.organizeImports.biome": "explicit"
    },
    "editor.defaultFormatter": "biomejs.biome",
    "editor.tabSize": 2
  },

  // Ruff
  "ruff.importStrategy": "useBundled",
  "ruff.lint.run": "onSave",
  "ruff.format.args": ["--line-length", "120"],
  "[python]": {
    "editor.defaultFormatter": "charliermarsh.ruff",
    "editor.codeActionsOnSave": {
      "source.fixAll": "explicit",
      "source.organizeImports": "explicit"
    },
    "editor.tabSize": 4
  },

  // Python
  "python.analysis.typeCheckingMode": "standard",
  "python.languageServer": "Pylance",
  "python.testing.pytestEnabled": true,

  // IntelliCode
  "vsintellicode.typescript.completionsEnabled": true
}
```

To apply these settings:

1. Open the Command Palette (Ctrl+Shift+P or Cmd+Shift+P on macOS)
2. Type "Preferences: Open Settings (JSON)"
3. Paste the above settings into your `settings.json` file

Feel free to adjust these settings according to your preferences and project requirements.

## Usage

Once installed and configured, you can start using the extensions right away in your AWS CDK projects. The extensions will automatically enhance your development environment with features like code completion, linting, formatting, and more.

For specific usage instructions for each extension, please refer to their individual documentation.

---
## Feedback and Contributions

If you have any feedback or suggestions for improving this extension pack, please open an issue on the [GitHub repository](https://github.com/towardsthecloud/vscode-cdk-extension-pack/issues). Contributions are always welcome!

Happy coding with AWS CDK!

## Author

[Danny Steenman](https://towardsthecloud.com/about)

[![](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/towardsthecloud)
[![](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/dannysteenman)
[![](https://img.shields.io/badge/GitHub-2b3137?style=for-the-badge&logo=github&logoColor=white)](https://github.com/towardsthecloud)
