# Personal Website

## Instructions

This is my personal website built using the [Zine](https://zine-ssg.io) static site generator.

To run it locally in your Web browser, you can install Zine, run the command, and go to [http://localhost:1990/](http://localhost:1990/):

```bash
zine
```

### Alternative

The website is served through Cloudflare Pages. To go to the website, open your Web browser and navigate to [https://jaudiger.dev/](https://jaudiger.dev/).

## CI / CD

The CI/CD pipeline is configured using GitHub Actions. The workflow is defined in the [`.github/workflows`](.github/workflows) folder:

- Static Analysis (GitHub Actions)
- Deployment

Additionally, Dependabot is configured to automatically update dependencies (GitHub Actions, Terraform providers).

## Repository configuration

The settings of this repository are managed from the [gitops-deployments](https://github.com/jaudiger/gitops-deployments) repository using Terraform. The actual configuration applied is located in the Terraform module [`modules/github-repository`](https://github.com/jaudiger/gitops-deployments/tree/main/modules/github-repository).
