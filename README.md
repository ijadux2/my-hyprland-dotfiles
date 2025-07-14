# Hyprland Configuration README

Welcome to my Hyprland configuration repository! This README will guide you through the setup and customization of my Hyprland environment.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Keybindings](#keybindings)
- [Themes](#themes)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Hyprland is a dynamic tiling Wayland compositor that offers a modern and efficient desktop experience. This configuration aims to enhance usability and aesthetics, providing a smooth workflow.

## Requirements

Before you begin, ensure you have the following installed:

- [Hyprland](https://github.com/hyprwm/Hyprland)
- [Wayland](https://wayland.freedesktop.org/)
- [Sway utilities](https://github.com/swaywm/sway)
- [Other dependencies](#other-dependencies)

### Other Dependencies

- `wlroots`
- `waybar`
- `rofi`
- `picom` (for compositing)
- `dunst` (for notifications)

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/ijadux2/my-hyprland-dotfiles.git
   ```

2. Navigate to the cloned directory:

   ```bash
   cd hyprland-config
   ```

3. Copy the configuration files to the appropriate directories:

   ```bash
   cp -r * ~/.config/hypr/
   ```

4. Install any required dependencies using your package manager.

## Configuration

The main configuration file is located at `~/.config/hypr/hyprland.conf`. You can customize various settings, including:

- **Window management**: Adjust tiling behavior, gaps, and floating windows.
- **Appearance**: Set colors, fonts, and other UI elements.
- **Autostart applications**: Define applications that should start automatically.

### Example Configuration

Here’s a snippet of a sample configuration:

```ini
# Window management
window_gap = 10
floating = [ "firefox", "gnome-terminal" ]

# Appearance
background = #282a36
foreground = #f8f8f2
```

## Keybindings

Keybindings can be customized in the `hyprland.conf` file. Here are some default keybindings:

- `Mod + Enter`: Open terminal
- `Mod + D`: Open application launcher
- `Mod + H`: Move focus left
- `Mod + J`: Move focus down
- `Mod + K`: Move focus up
- `Mod + L`: Move focus right

## Themes

You can customize the look of your Hyprland environment by using themes. Place your theme files in the `~/.config/hypr/themes/` directory and reference them in your `hyprland.conf`.

## Troubleshooting

If you encounter issues, consider the following steps:

1. Check the logs for errors:
   ```bash
   journalctl -xe | grep hyprland
   ```

2. Ensure all dependencies are installed.
3. Review your configuration files for syntax errors.

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to customize this README further to suit your specific configuration and preferences!
