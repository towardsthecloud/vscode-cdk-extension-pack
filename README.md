# AWS CDK Extension Pack

[![Version](https://img.shields.io/visual-studio-marketplace/v/dannysteenman.aws-cdk-extension-pack?color=374151&label=Visual%20Studio%20Marketplace&labelColor=000&logo=visual-studio-code&logoColor=0098FF)](https://marketplace.visualstudio.com/items?itemName=dannysteenman.aws-cdk-extension-pack)
[![Installs](https://img.shields.io/visual-studio-marketplace/i/dannysteenman.aws-cdk-extension-pack 'Currently Installed')](https://marketplace.visualstudio.com/items?itemName=dannysteenman.aws-cdk-extension-pack)
[![Rating](https://img.shields.io/visual-studio-marketplace/stars/dannysteenman.aws-cdk-extension-pack)](https://marketplace.visualstudio.com/items?itemName=dannysteenman.aws-cdk-extension-pack)

This is a collection of extensions that I've curated in this vscode extension pack to help you build, deploy and manage your AWS CDK applications.

> [!TIP]
> **Launch Faster on AWS and Become Fully Secure From Day One!** Our AWS Landing Zone Foundation service helps B2B companies achieve SOC 2 compliance 90% faster,  redirect 30% of engineering time back to product development all while eliminating the six-figure cost of specialized cloud engineers. so you can focus on shipping your product, instead of worrying about managing your infrastructure on AWS.
>
> [Schedule a free introduction call](https://towardsthecloud.com/contact) to discover how we can deliver 10x the value of securing and building your infrastructure on AWS for a fraction of the cost of a full-time cloud engineer.

<details><summary>☁️ <strong>Learn more about our unique AWS Foundation Service</strong></summary>

<br/>

Is AWS complexity draining your engineering resources? Most B2B startups and growing businesses struggle with overwhelming configuration options, time-consuming compliance requirements, and diverting valuable developer talent away from core product development. Without specialized AWS expertise, you risk security vulnerabilities, mounting technical debt, and delayed time-to-market. All while your competitors race ahead.

Traditional AWS consultancies only compound this problem. They're incentivized to bill by the hour, extending projects indefinitely rather than focusing on your business outcomes. We take the opposite approach. Our fixed-price subscription model proves how confident we are in delivering results, not just billable hours. We succeed when you succeed, aligning our incentives with your growth rather than your AWS complexity.

## Our Solution: Enterprise-Grade AWS Foundation

We deliver an enterprise-grade AWS Landing Zone built entirely in AWS CDK coupled with a support and consultacy foundation that grows with your business needs. Here's what we'll deliver to you:

### We deploy a [Secure and Compliant Landing Zone](https://towardsthecloud.com/services/aws-landing-zone)
- Multi-account architecture with proper security boundaries
  - Achieves a **100% score on the industry-standard [CIS AWS Foundation Benchmark](https://docs.aws.amazon.com/securityhub/latest/userguide/cis-aws-foundations-benchmark.html)**
  - **Achieves a 96% rating on AWS's own [foundational security best practices](https://docs.aws.amazon.com/securityhub/latest/userguide/fsbp-standard.html)**
- Setup entirely using AWS CDK (Infrastructure as Code)
- Budget monitoring and notifications across all accounts
- Deploy changes quickly through GitHub Actions
- We're continuously adding new features as listed on our [Roadmap](https://github.com/towardsthecloud/aws-cdk-landing-zone-roadmap)

### We upskill and accelerate your Developers
- They gain access to our library of ready-to-use, security-hardened AWS CDK components
- They receive guidance on how to utilize AWS best practices for your architecture so you avoid technical debt later on

### We monitor and maintain the multi-account setup & provide ongoing support
- Gain new Landing Zone features once they're released and get free maintenance and security updates
- Get priority support through Slack/Teams whenever you need assistance with infrastructure challenges
- We proactively do quarterly [security](https://towardsthecloud.com/services/aws-security-review) and [cost optimization](https://towardsthecloud.com/services/aws-cost-optimization) assessments to verify AWS account compliance and provide advice to reduce your AWS bill

### What This Means For Your Business
- **30% Lower TCO**: Cut your Total Cost of Ownership (TCO) by up to 30% through right-sized resources and architectural optimization while eliminating the $150K+ annual cost of a specialized AWS hire
- **Close Enterprise Deals Faster**: Win enterprise clients with SOC2 compliance ready in weeks instead of months - our clients report 50% faster sales cycles with security-conscious customers
- **Unleash Your Development Team**: Redirect up to 30% of engineering time from infrastructure back to revenue-generating product features with our pre-built, compliant components
- **Scale Without Infrastructure Headaches**: Grow from startup to enterprise without ever rebuilding your foundation - our architecture scales seamlessly from your first customer to your millionth

We deliver all of this as a [simple subscription service](https://towardsthecloud.com/pricing). No large upfront costs, no lock-in. You'll essentially get a solid and secure landing zone foundation + a decade of AWS expertise without having to hire a full-time Cloud Engineer.

<a href="https://towardsthecloud.com/contact"><img alt="Schedule a free introduction call" src="https://img.shields.io/badge/schedule%20a%20free%20introduction%20call-success.svg?style=for-the-badge"/></a>
</details>

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
