# pyRevit Tools for Notepad++
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

A pyRevit extension providing a suite of tools for Revit users who utilize Notepad++ for scripting, log analysis, or configuration management. This extension bridges the gap between the Revit environment and the powerful text-editing capabilities of Notepad++.

## Features

Export: Quickly send Revit data, such as family parameters, Forma cache file paths, and project fill patterns, to Notepad++ with one click.

Log Viewer: Open Revit and pyRevit logs directly to Notepad++ for advanced filtering and searching.

Config Management: Easily edit pyRevit_config.ini and other XML, json, and ini configuration files with syntax highlighting.

## Installation

### The Easy Way (pyRevit CLI)

If you have pyRevit installed, run the following command in PowerShell:

``` powershell
pyrevit extend ui pyMAWtoolsforNPP https://github.com/mawdesign/pyRevit-tools-for-npp.git
```

### The Manual Way

1. Clone this repository into your pyRevit extensions folder: `git clone https://github.com/mawdesign/pyRevit-tools-for-npp.git pyMAWtoolsforNPP.extension`
2. Add `%APPDATA%\pyRevit\Extensions\RevitToolsNPP.extension` to `%APPDATA%\pyRevit\pyRevit_config.ini`

## Usage

Once installed, a new tab labeled "pyMAW" (or a new Notepad++ panel under your existing pyMAW tab) will appear in the Revit Ribbon.

## License

This work is licensed under a Creative Commons Attribution 4.0 International License (CC-BY-4.0).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue for bug reports and feature requests.
