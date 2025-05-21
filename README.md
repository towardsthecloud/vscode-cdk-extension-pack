# AWS CDK Extension Pack

[![Version](https://img.shields.io/visual-studio-marketplace/v/dannysteenman.aws-cdk-extension-pack?color=374151&label=Visual%20Studio%20Marketplace&labelColor=000&logo=visual-studio-code&logoColor=0098FF)](https://marketplace.visualstudio.com/items?itemName=dannysteenman.aws-cdk-extension-pack)
[![Installs](https://img.shields.io/visual-studio-marketplace/i/dannysteenman.aws-cdk-extension-pack 'Currently Installed')](https://marketplace.visualstudio.com/items?itemName=dannysteenman.aws-cdk-extension-pack)
[![Rating](https://img.shields.io/visual-studio-marketplace/stars/dannysteenman.aws-cdk-extension-pack)](https://marketplace.visualstudio.com/items?itemName=dannysteenman.aws-cdk-extension-pack)

This is a collection of extensions that I've curated in this vscode extension pack to help you build, deploy and manage your AWS CDK applications.

> [!TIP]
> **AWS Done Right: Ship Faster, More Securely, at Lower Cost!** Our [AWS CDK Landing Zone Service](https://towardsthecloud.com) helps B2B startups & enterprises achieve SOC 2 compliance 90% faster, reclaim 30% of developer capacity for product innovation while eliminating six-figure Cloud Engineering costs.
>
> Discover how we deliver 10x AWS infrastructure value while cutting costs.
>
> <a href="https://towardsthecloud.com/contact"><img alt="Book your free intro call" src="https://img.shields.io/badge/book%20your%20free%20intro%20call-success.svg?style=for-the-badge"/></a>
>
> <details><summary>☁️ <strong>Learn more how we help businesses succeed on AWS Cloud...</strong></summary>
>
><br/>
>
> AWS promises simplicity but delivers complexity. Businesses struggle with security risks and compliance requirements that divert developers from core product work.
>
> Without AWS expertise, you face vulnerabilities, technical debt, and market delays while competitors race ahead.
>
> Traditional consultancies worsen this by prioritizing billable hours over outcomes.
>
> We take the opposite approach, focusing exclusively on business outcomes by eliminating AWS complexity, accelerating your developers, and securing your infrastructure through:
>
> ### Deploying a [Secure Landing Zone](https://towardsthecloud.com/services/aws-landing-zone)
> - Multi-account architecture with strict security boundaries
>   - **100% score** on [CIS AWS Foundation Benchmark](https://docs.aws.amazon.com/securityhub/latest/userguide/cis-aws-foundations-benchmark.html)
>   - **96% rating** on [AWS foundational security best practices](https://docs.aws.amazon.com/securityhub/latest/userguide/fsbp-standard.html)
> - Manage user access securely on AWS via Single Sign-On (SSO)
> - Full AWS CDK implementation (Infrastructure as Code)
> - Multi-region deployments supported
> - Cross-account monitoring and security alerts
> - View our [Roadmap](https://github.com/towardsthecloud/aws-cdk-landing-zone-roadmap) for all implemented and upcoming features
>
> ### Upskilling and accelerating your developers
> - They get access to our production-ready, security-hardened AWS CDK components
> - They receive AWS best practices guidance to prevent technical debt
>
> ### Providing support and maintenance
> - Landing Zone gets updates and security patches
> - Priority Slack/Teams support for infrastructure challenges
> - Quarterly [security](https://towardsthecloud.com/services/aws-security-review) and [cost optimization](https://towardsthecloud.com/services/aws-cost-optimization) assessments to stay compliant and reduce AWS costs
>
> ## What This Means For Your Business
> - **30% Lower TCO**: Cut Total Cost by 40% through right-sized resources while eliminating the $150K+ cost of a specialized AWS hire.
> - **Accelerate Development**: Redirect 30% of engineering time from infrastructure to revenue-generating features with pre-built, compliant CDK components.
> - **Compliance-Ready Infrastructure**: Meet security requirements from day one with architecture that [speeds up audit preparation by 90%](https://towardsthecloud.com/blog/aws-landing-zone-case-study-accolade) for SOC 2, HIPAA, and other security frameworks.
>
> All of this is included in a [fixed monthly subscription](https://towardsthecloud.com/pricing). No lock-in, no large upfront costs, just predictable monthly pricing.
>
> Book a free call to see how we deliver 10x AWS infrastructure value at a fraction of a Cloud Engineer's cost.
>
> <a href="https://towardsthecloud.com/contact"><img alt="Book your free introduction call" src="https://img.shields.io/badge/book%20your%20free%20introduction%20call-success.svg?style=for-the-badge"/></a>
> </details>

## Included Extensions

This extension pack includes the following VS Code extensions:

1. **AWS Toolkit for Visual Studio Code**: Provides support for developing AWS applications
2. **Biome**: A performant linter, formatter, and more for JavaScript, TypeScript, and JSON
3. **Ruff**: An extremely fast Python linter and code formatter
4. **CDK Snippets**: Code snippets for AWS CDK development
5. **AWS IAM Actions Snippets**: Adds autocomplete and snippets for all AWS IAM policy actions
6. **AWS IAM Service Principal Snippets**: Autocompletion for AWS service principals.
7. **Draw.io Integration**: Integrates Draw.io diagrams into VS Code
8. **Docker**: Makes it easy to create, manage, and debug containerized applications
9. **Python**: IntelliSense, linting, debugging, and more for Python
10. **Pylance**: Fast, feature-rich language support for Python
11. **IntelliCode API Usage Examples**: AI-assisted code examples for API usage
12. **IntelliCode**: AI-assisted development features

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
