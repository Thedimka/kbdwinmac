# Windows Mac Keyboard Layout

A Windows keyboard layout that mimics Mac OS keyboard behavior, optimized for Russian/English input. Ideal for users who frequently switch between Mac and Windows systems.

## Features

- Mac-style (Currently only Russian) keyboard layout for Windows
- Familiar key positions for Mac users
- Support for both Windows 10 and 11
- Simple installer with visual preview

## Prerequisites

- Windows 10 or Windows 11
- Administrative privileges (required for keyboard layout installation)

## Installation

1. Download the latest installer from the [Releases](https://github.com/yourusername/kbdwinmac/releases) page
2. Run the installer
3. Follow the installation wizard
4. Restart your computer (optional, but recommended)
5. Select the "Russian (Mac)" layout in Windows language settings

## Building from Source

### Prerequisites

- Windows 10/11
- WiX Toolset v5+
- Visual Studio (for building the DLL)

### Build Steps

1. Clone the repository:
```cmd
git clone https://github.com/yourusername/kbdwinmac.git
```

2. Build the installer:
```cmd
cd kbdwinmac
wix build install-kbdwinmac.wxs -ext WixToolset.UI.wixext
```

## Project Structure

```
kbdwinmac/
├── DLLs/              # Compiled keyboard layout DLLs
├── src/               # Source code for the keyboard layout
├── layout.bmp         # Layout preview image
└── install-kbdwinmac.wxs  # WiX installer configuration
```

## License

[MIT License](LICENSE)

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request