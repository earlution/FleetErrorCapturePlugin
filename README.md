
# FleetErrorCapturePlugin

FleetErrorCapturePlugin is an open-source plugin for JetBrains' Fleet IDE that captures all code errors, warnings, and weak warnings in a single file. Instead of manually copying each error or warning, this plugin automates the process, saving developers time, especially when working with AI-powered tools like Claude or ChatGPT to debug their code.

## Features

- Automatically captures all error, warning, and weak warning information from Fleet's code analysis.
- Exports the captured data into a structured file (JSON or plain text), including:
  - Line number
  - Error/Warning type
  - Full error/warning message
- Easy-to-use interface to export and manage the captured error log.

## Getting Started

### Prerequisites

To get started, ensure you have the following:
- **Fleet IDE** (macOS version)
- **Plugin SDK** for Fleet IDE (to be confirmed based on Fleet's plugin architecture)

### Installation

1. Clone the repository:
   \`\`\`bash
   git clone https://github.com/yourusername/FleetErrorCapturePlugin.git
   cd FleetErrorCapturePlugin
   \`\`\`
2. Follow the instructions for building Fleet IDE plugins (coming soon).
3. Once installed, the plugin will run in the background and automatically capture errors/warnings.

### Usage

1. Once installed, you’ll have access to a new **Export Errors** option in Fleet's interface.
2. Click on this option to save all the current errors and warnings in a chosen format (JSON or plain text).
3. The file will include the line numbers, types (Error/Warning/Weak Warning), and detailed messages for each issue.

### Example

#### JSON Format
\`\`\`json
{
  "errors": [
    {
      "line": 42,
      "type": "Error",
      "message": "SyntaxError: Unexpected token"
    },
    {
      "line": 58,
      "type": "Warning",
      "message": "Unused variable"
    }
  ]
}
\`\`\`

#### Plain Text Format
\`\`\`
Line 42 - Error: SyntaxError: Unexpected token
Line 58 - Warning: Unused variable
\`\`\`

## Roadmap

- **v0.1.0**: Initial release capturing and exporting errors/warnings to a file.
- **v0.2.0**: Add support for different platforms (Windows, Linux).
- **v0.3.0**: Improve the user interface and introduce customizable export formats.

## Contributing

We welcome contributions from the community! To get started:
1. Fork the repository.
2. Create a new branch for your feature (\`git checkout -b feature/your-feature\`).
3. Submit a pull request.

For more detailed guidelines, see the \`CONTRIBUTING.md\` file.

## License

This project is licensed under the MIT License - see the \`LICENSE.md\` file for details.
