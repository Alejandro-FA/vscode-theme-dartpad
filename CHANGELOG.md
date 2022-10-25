# Changelog

All notable changes to the ["vscode-theme-dartpad"](https://marketplace.visualstudio.com/items?itemName=Alejandro-FA.vscode-theme-dartpad) extension will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.4.0] - 2022-10-25
### Added
- Syntax highlighting rules have now been tested with Markdown, Python, Java and C++. All these languages should now follow the same logic when it comes to highlighting colors.
### Changed
- Semantic highlighting has been tweaked to depend as much as possible on the [predefined TextMate scope mappings](https://code.visualstudio.com/api/language-extensions/semantic-highlight-guide#predefined-textmate-scope-mappings). This should improve consistency and mantainability, although some tokens might be of different color now.
### Removed
- All language-specific syntax highlighting rules (except Markdown) have been removed. Some of the affected scopes have been moved to the corresponding generic rules, while others are no longer taken into consideration. This change should improve maintainability and consistency throughout multiple languages.

## [0.3.0] - 2022-10-16
### Added
- Changelog.
- MIT License.

### Changed
- Docstrings (`string.quoted.docstring`) now use the same color as comments (`#909cc3`). Previously used color was the same as strings (`#fa557d`).
- `variable.language` token color changed to `#4fe191` to match DartPad. Language specific settings of this token have been removed.
- Black elements of the UI have been changed to use a slightly brighter color (`#0a0f16`). The goal of this change is to achieve a less "contrasty" feel.

### Fixed
- Fix typos in README.md.
