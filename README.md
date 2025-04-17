# AWS CDK Extension Pack

[![Version](https://img.shields.io/visual-studio-marketplace/v/dannysteenman.aws-cdk-extension-pack?color=374151&label=Visual%20Studio%20Marketplace&labelColor=000&logo=visual-studio-code&logoColor=0098FF)](https://marketplace.visualstudio.com/items?itemName=dannysteenman.aws-cdk-extension-pack)
[![Installs](https://img.shields.io/visual-studio-marketplace/i/dannysteenman.aws-cdk-extension-pack 'Currently Installed')](https://marketplace.visualstudio.com/items?itemName=dannysteenman.aws-cdk-extension-pack)
[![Rating](https://img.shields.io/visual-studio-marketplace/stars/dannysteenman.aws-cdk-extension-pack)](https://marketplace.visualstudio.com/items?itemName=dannysteenman.aws-cdk-extension-pack)

This is a collection of extensions that I've curated in this vscode extension pack to help you build, deploy and manage your AWS CDK applications.

> [!TIP]
> Struggling with AWS complexity or stuck on-premise? Let's transform your cloud journey.
>
> [Schedule a call with me](https://towardsthecloud.com/contact) to find out how I can enhance your existing AWS setup or guide your journey from on-premise to the Cloud.
>
> <details><summary>☁️ <strong>Discover more about my one-person business: Towards the Cloud</strong></summary>
>
> <br/>
>
> Hi, I'm Danny – AWS expert and founder of [Towards the Cloud](https://towardsthecloud.com). With over a decade of hands-on experience, I specialized myself in deploying well-architected, highly scalable and cost-effective AWS Solutions using Infrastructure as Code (IaC).
>
> #### When you work with me, you're getting a package deal of expertise and personalized service:
>
> - **AWS CDK Proficiency**: I bring deep AWS CDK knowledge to the table, ensuring your infrastructure is not just maintainable and scalable, but also fully automated.
> - **AWS Certified**: [Equipped with 7 AWS Certifications](https://www.credly.com/users/dannysteenman/badges), including DevOps Engineer & Solutions Architect Professional, to ensure best practices across diverse cloud scenarios.
> - **Direct Access**: You work with me, not a team of managers. Expect quick decisions and high-quality work.
> - **Tailored Solutions**: Understanding that no two businesses are alike, I Custom-fit cloud infrastructure for your unique needs.
> - **Cost-Effective**: I'll optimize your AWS spending without cutting corners on performance or security.
> - **Seamless CI/CD**: I'll set up smooth CI/CD processes using GitHub Actions, making changes a breeze through Pull Requests.
>
> *My mission is simple: I'll free you from infrastructure headaches so you can focus on what truly matters – your core business.*
>
> Ready to unlock the full potential of AWS Cloud?
>
> <a href="https://towardsthecloud.com/contact"><img alt="Schedule your call" src="https://img.shields.io/badge/schedule%20your%20call-success.svg?style=for-the-badge"/></a>
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
