# YAML-JS Build Tools Monorepo

This repository contains a suite of build tools for use in yaml-js projects. It includes GitHub Actions designed to streamline and automate project workflows, ensuring consistent and efficient continuous integration and deployment.

## Structure

The repository is organized as follows:

```
/.github/
└── workflows/
/github-actions
└── update-package-version/
└── [future-action]/
/github-actions-src
└── lib
    └── update-package-version/
    └── [future-action]/
└── src
    └── update-package-version/
    └── [future-action]/
```

- **`.github/workflows/`**: Contains workflow files specific to this repository, defining how GitHub Actions are run within the project.
- **`github-actions/`**: Contains individual GitHub Action definitions. Each action is organized within its own directory.
- **`github-actions-src/`**: Houses the packages and scripts used to develop and maintain the GitHub Actions.

## Tools

This repository includes a variety of tools aimed at improving the development, testing, and deployment processes for yaml-js projects.

### GitHub Actions

![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/yaml-js/build/build.yml)
![Sonar Quality Gate](https://img.shields.io/sonar/quality_gate/org.yaml-js.build-toolkit?server=https%3A%2F%2Fsonarcloud.io)
![Sonar Tech Debt](https://img.shields.io/sonar/tech_debt/org.yaml-js.build-toolkit?server=https%3A%2F%2Fsonarcloud.io)
![Sonar Coverage](https://img.shields.io/sonar/coverage/org.yaml-js.build-toolkit?server=https%3A%2F%2Fsonarcloud.io)
![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/yaml-js/build)

A collection of GitHub Actions developed to facilitate continuous integration (CI) and continuous deployment (CD) tasks for yaml-js projects.

#### Available Actions

##### 1. Update package.json Version

- **Description**: This action updates the `version` field in the `package.json` file, replacing it with the version specified by a Git tag. It is useful for automating version management in CI/CD pipelines.
- **Directory**: `github-actions/update-package-version/`
- **[Usage Instructions](github-actions/update-package-version/README.md)**: Detailed usage instructions can be found in the action's dedicated `README.md` file.

#### [Future Actions]

- **Description**: Placeholder for future GitHub Actions that will be added to this repository.
- **Directory**: `github-actions/[future-action]/`
- **Usage Instructions**: Each new action will have its own `README.md` file with detailed usage instructions.

## Contributing

Contributions are welcome! If you have ideas for new tools or improvements to existing ones, feel free to open an issue or submit a pull request.

### Adding a New Action

1. Create a new directory under github-actions/ with the name of your action.
2. Develop your action and include a README.md file with clear usage instructions.
3. Update the root README.md file to include your new action in the Available Actions section.

## License

This repository is licensed under the MIT License. Please look at the [LICENSE](./LICENSE) file for more details.


