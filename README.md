# PatchPanelProject
PatchPanel - Patching Schedule tool V1  
# Patch Panel Manager

A web-based application for managing network patch panel configurations, designed by Meta Eagle for efficient documentation and organisation of network infrastructure.

## Overview

Patch Panel Manager is a client-side web application that allows network professionals to create, manage, and document patch panel configurations across multiple projects and locations. All data is stored locally in the browser, ensuring privacy and eliminating the need for external servers.

**Note**: This tool was originally written for an internal Meta Eagle project in August 2023 and is not actively maintained or kept up to date. It is provided as-is for testing and educational purposes.

## Features

- **Project Management**: Create and manage multiple projects, each with its own configuration
- **Room Organisation**: Organise patch panels by rooms or physical locations
- **VLAN & Switch Management**: Define VLANs and switches per project for easy configuration
- **Port Configuration**: Configure individual ports with switch connections, VLANs, and notes
- **Visual & Summary Views**: View patch panels both visually and in detailed summary tables
- **Export Capabilities**: 
  - Export projects to JSON for backup and sharing
  - Export to CSV for spreadsheet analysis
  - Generate HTML site reports for documentation
- **Import Functionality**: Import previously exported projects
- **Local Storage**: All data stored locally in browser - no server required

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- No installation or server setup required

### Usage

1. Open `index.html` in your web browser or visit the live site at: https://lee-robinson.github.io/PatchPanelProject/
2. Click "Create New Project" to start a new project
3. Define your rooms, VLANs, and switches
4. Add patch panels to rooms
5. Click on individual ports to configure connections
6. Export your project for backup or sharing

## Detailed Instructions

### Creating a Project

1. Click the "Create New Project" button
2. Enter a project name
3. Add rooms (e.g., "Server Room", "IDF 1", "MDF")
4. Add VLANs (e.g., "Data", "Voice", "Management")
5. Add switches (e.g., "Core-SW-01", "Access-SW-02")
6. Click "Save Project"

### Managing Patch Panels

1. Select a project from the dropdown
2. Within each room, click "Add Patch Panel"
3. Click on the patch panel name to edit its name and description
4. Click on individual ports (1-24) to configure them

### Configuring Ports

When configuring a port, you can specify:
- **Connected to SwitchPort**: The port on the switch this connects to
- **VLAN**: Select from your predefined VLANs
- **Switch**: Select from your predefined switches
- **Notes**: Any additional information about the connection

### Exporting and Importing

- **Export Project**: Downloads both a CSV file and a JSON file
  - JSON file can be imported back into the application
  - CSV file can be opened in Excel or other spreadsheet software
- **Generate Site Report**: Creates a formatted HTML document
- **Import Project**: Load a previously exported JSON file

## Data Storage

All project data is stored in your browser's localStorage. This means:

- Data persists between browser sessions
- Data is specific to the browser and device you're using
- No data is sent to external servers
- Storage limit is approximately 5-10 MB, depending on your browser

**Important**: Regularly export your projects to ensure you have backups, as clearing browser data will delete all stored projects.

## Browser Compatibility

The application works with all modern browsers that support:
- HTML5
- CSS3
- JavaScript ES6+
- localStorage API

Tested browsers:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Network Design Example

The application was designed with the following network structure in mind:

- **Data VLAN**: 10.0.0.0/22 (1022 hosts)
- **Voice VLAN**: 10.0.4.0/24 (254 hosts)
- **CCTV VLAN**: 10.0.5.0/24 (254 hosts)
- **Printers VLAN**: 10.0.6.0/24 (254 hosts)
- **Servers VLAN**: 10.0.7.0/24 (254 hosts)
- **Workstations VLAN**: 10.0.8.0/24 (254 hosts)

## Screenshots

*(You can add screenshots of the application here once it's deployed)*

## Limitations

- Data is stored locally only - not synchronised across devices
- Browser storage limits may restrict very large projects
- No collaboration features for multi-user environments
- **This project is not actively maintained** - written for an internal project in August 2023

## Disclaimer

This application is provided by Meta Eagle for testing and development purposes only. This tool was originally written for an internal Meta Eagle project in August 2023 and is not actively maintained or kept up to date. While we strive for accuracy and reliability, we cannot be held liable for any bugs in the application or for the accuracy of generated reports. Users who choose to utilise this tool for professional purposes do so at their own risk. We encourage users to regularly export and back up their data to prevent any potential loss of information.

## Contributing

This is an open-source project. While not actively maintained, contributions, issues, and feature requests are welcome and appreciated!

## License

This project is open source and available under the [MIT License](LICENSE).

## Author

**Meta Eagle**
- Website: [https://metaeagle.co.uk](https://metaeagle.co.uk)
- Repository: [https://github.com/Lee-Robinson/PatchPanelProject](https://github.com/Lee-Robinson/PatchPanelProject)


## Version History

- **v1.0.0** (August 2023) - Initial release
  - Project and room management
  - Patch panel configuration (24 ports per panel)
  - Export/Import functionality
  - Site report generation
  - Visual port representation with summary tables

## Support

For issues, questions, or suggestions, please open an issue on the GitHub repository. Please note that as this is not an actively maintained project, responses may be delayed or limited.

## Roadmap

Potential future enhancements (if development resumes):
- Support for different patch panel sizes (12, 48 ports)
- Print-friendly views
- Cable labeling templates
- Integration with network management tools
- Dark/Light theme toggle

---

**Note**: This tool was written for an internal project in August 2023 and is not kept up to date. Remember to export your projects regularly as backups. All data is stored locally in your browser.
