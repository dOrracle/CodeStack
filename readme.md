# CodeStack

A simple desktop application for viewing multiple code inside of multiple files simultaneously, designed to enhance developer productivity.

## Features

- Multi-file viewing capability
- copy individual file code or complete multiple file printout.
- Cross-platform support (Windows, macOS, Linux)
- Built with Electron and React for a modern, responsive interface

## Prerequisites

Before you begin, ensure you have installed:
- Node.js (v16 or higher)
- npm (v8 or higher)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/dOrracle/CodeStack.git
cd CodeStack
```

2. Install dependencies:
```bash
npm install
```

## Development

To run the application in development mode:
```bash
npm start
```

## Building

To build the application for distribution:
```bash
npm run build
```

Build outputs will be available in the `dist` directory.

### Build Requirements

For macOS builds:
- Place a 1024x1024px PNG icon in `build/icon.png`
- XCode Command Line Tools installed

For Windows builds:
- Windows or appropriate cross-compilation setup
- (Optional) Wine for building on non-Windows platforms

## Project Structure

```
codestack/
├── main.js           # Main Electron process
├── src/              # Application source code
├── build/            # Build resources
│   └── icon.png      # Application icon
├── package.json      # Project configuration
└── README.md         # This file
```

## Configuration

The application can be configured through `package.json`. Key configuration options are found in the `build` section:

```json
{
  "build": {
    "appId": "com.jason.codestack",
    "productName": "CodeStack",
    "mac": {
      "category": "public.app-category.developer-tools",
      "target": ["dmg", "zip"]
    }
  }
}
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Author

jason@jasonorr.info

## Acknowledgments

- Built with [Electron](https://www.electronjs.org/)
- UI powered by [React](https://reactjs.org/)
- Claude powered by Sonnet 3.5

## Support

For support, please open an issue in the GitHub repository.

## Roadmap

- [ ] Add syntax highlighting
- [ ] Implement search functionality
- [ ] Add file comparison features
- [ ] Support for custom themes
- [ ] Add plugin system

---

**Note:** This project is under active development. Features and documentation may change frequently.