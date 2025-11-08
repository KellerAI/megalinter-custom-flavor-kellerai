# MegaLinter Custom Flavor: KellerAI_MegaLinter

A pre-built custom MegaLinter flavor with a curated set of linters. This repository tracks upstream MegaLinter releases and provides a ready-to-use GitHub Action with our selected linters.

Maintained on <https://github.com/KellerAI/megalinter-custom-flavor-kellerai> by Jonathan Bowe

## Embedded linters

- [BASH_SHELLCHECK](https://megalinter.io/latest/descriptors/bash_shellcheck/)
- [DOCKERFILE_DOCKERFILELINT](https://megalinter.io/latest/descriptors/dockerfile_dockerfilelint/)
- [DOCKERFILE_HADOLINT](https://megalinter.io/latest/descriptors/dockerfile_hadolint/)
- [EDITORCONFIG_EDITORCONFIG_CHECKER](https://megalinter.io/latest/descriptors/editorconfig_editorconfig_checker/)
- [ENV_DOTENV_LINTER](https://megalinter.io/latest/descriptors/env_dotenv_linter/)
- [JAVASCRIPT_ES](https://megalinter.io/latest/descriptors/javascript_es/)
- [JAVASCRIPT_PRETTIER](https://megalinter.io/latest/descriptors/javascript_prettier/)
- [JAVASCRIPT_STANDARD](https://megalinter.io/latest/descriptors/javascript_standard/)
- [JSON_JSONLINT](https://megalinter.io/latest/descriptors/json_jsonlint/)
- [JSON_NPM_PACKAGE_JSON_LINT](https://megalinter.io/latest/descriptors/json_npm_package_json_lint/)
- [JSON_PRETTIER](https://megalinter.io/latest/descriptors/json_prettier/)
- [JSON_V8R](https://megalinter.io/latest/descriptors/json_v8r/)
- [MAKEFILE_CHECKMAKE](https://megalinter.io/latest/descriptors/makefile_checkmake/)
- [MARKDOWN_MARKDOWNLINT](https://megalinter.io/latest/descriptors/markdown_markdownlint/)
- [MARKDOWN_MARKDOWN_LINK_CHECK](https://megalinter.io/latest/descriptors/markdown_markdown_link_check/)
- [MARKDOWN_MARKDOWN_TABLE_FORMATTER](https://megalinter.io/latest/descriptors/markdown_markdown_table_formatter/)
- [PYTHON_BANDIT](https://megalinter.io/latest/descriptors/python_bandit/)
- [PYTHON_BLACK](https://megalinter.io/latest/descriptors/python_black/)
- [PYTHON_ISORT](https://megalinter.io/latest/descriptors/python_isort/)
- [PYTHON_MYPY](https://megalinter.io/latest/descriptors/python_mypy/)
- [PYTHON_RUFF](https://megalinter.io/latest/descriptors/python_ruff/)
- [PYTHON_RUFF_FORMAT](https://megalinter.io/latest/descriptors/python_ruff_format/)
- [REPOSITORY_GITLEAKS](https://megalinter.io/latest/descriptors/repository_gitleaks/)
- [REPOSITORY_LS_LINT](https://megalinter.io/latest/descriptors/repository_ls_lint/)
- [REPOSITORY_SECRETLINT](https://megalinter.io/latest/descriptors/repository_secretlint/)
- [REPOSITORY_SEMGREP](https://megalinter.io/latest/descriptors/repository_semgrep/)
- [REPOSITORY_SYFT](https://megalinter.io/latest/descriptors/repository_syft/)
- [SPELL_PROSELINT](https://megalinter.io/latest/descriptors/spell_proselint/)
- [TYPESCRIPT_ES](https://megalinter.io/latest/descriptors/typescript_es/)
- [TYPESCRIPT_PRETTIER](https://megalinter.io/latest/descriptors/typescript_prettier/)
- [TYPESCRIPT_STANDARD](https://megalinter.io/latest/descriptors/typescript_standard/)
- [XML_XMLLINT](https://megalinter.io/latest/descriptors/xml_xmllint/)
- [YAML_PRETTIER](https://megalinter.io/latest/descriptors/yaml_prettier/)
- [YAML_V8R](https://megalinter.io/latest/descriptors/yaml_v8r/)
- [YAML_YAMLLINT](https://megalinter.io/latest/descriptors/yaml_yamllint/)

## How to use this custom flavor

### GitHub Action

This is a pre-built custom MegaLinter flavor - you don't need to build it yourself. Simply use it directly in your GitHub workflows.

In your workflow file (`.github/workflows/mega-linter.yml`), add:

```yaml
- name: MegaLinter
  uses: KellerAI/megalinter-custom-flavor-kellerai@main
```

That's it! This will automatically use our pre-built MegaLinter flavor with all the configured linters listed above.

## About this flavor

This is a pre-built custom MegaLinter flavor maintained as a GitHub Action. Users can directly use this flavor without any build steps.

**Key features**:
- **Ready to use**: No building required - just reference it in your GitHub Actions
- **Curated linter set**: Includes essential linters for JavaScript, TypeScript, Python, Docker, and more
- **Automatic version tracking**: Stays synchronized with upstream MegaLinter releases

## Version tracking

This repository automatically tracks upstream MegaLinter releases:

- **Daily checks**: The `check-new-megalinter-version` workflow runs daily to detect new MegaLinter versions
- **Automatic releases**: When a new version is found, a matching release is created in this repository
- **Version alignment**: The pre-built image is maintained separately and updated to match upstream versions
- **Release history**: Check the [Releases page](https://github.com/KellerAI/megalinter-custom-flavor-kellerai/releases) to see all tracked versions

The `megalinter-custom-flavor.yml` file defines which linters are included in this custom flavor.

[![MegaLinter is graciously provided by OX Security](https://raw.githubusercontent.com/oxsecurity/megalinter/main/docs/assets/images/ox-banner.png)](https://www.ox.security/?ref=megalinter)
