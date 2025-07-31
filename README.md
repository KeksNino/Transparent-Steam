# Steam Transparent

Adwaita for Steam custom css to make steam ui transparent

<img src="/home/user/.config/Typora/typora-user-images/image-20250801002029147.png" alt="image-20250801002029147" style="zoom:25%;" /><img src="/home/user/.config/Typora/typora-user-images/image-20250801002045065.png" alt="image-20250801002045065" style="zoom:25%;" />

## Requirements

* [Python 3](https://www.python.org/downloads/)
* The skin is created and tested mostly on the Linux version of Steam. Steam's new UI has largely unified platform differences, so other platforms should work, but are not a priority.

## Installation

### With installer script

```bash
git clone https://github.com/tkashkin/Adwaita-for-Steam
cd Adwaita-for-Steam
./install.py --custom-css
```

#### Arguments

| Argument                | Short | Required Values                                          | Description                                      |
| ----------------------- | ----- | -------------------------------------------------------- | ------------------------------------------------ |
| --help                  | -h    |                                                          | Show help message                                |
| --list-options          | -l    |                                                          | List available themes and extras                 |
| --font                  | -f    | adwaita / cantarell                                      | Change font family                               |
| --windowcontrols-theme  |       | auto / adwaita / breeze / windows / macos                | Change window control buttons style              |
| --windowcontrols-layout |       | auto / gnome / pantheon / windows / macos / \[custom]    | Change window control buttons position and order |
| --custom-css            |       |                                                          | Enable [custom css](/custom)                     |
| --extras                | -e    | [Extra](adwaita/extras)                                  | Enable one or multiple theme extras              |
| --target                | -t    | linux / windows / macos / flatpak / snap / \[custom dir] | Choose target location for install               |
| --uninstall             | -u    |                                                          | Uninstall theme                                  |

#### Example Usage

```bash
# List options
./install.py -l
# Install with customizations
./install.py --custom-css -e login/hide_qr -e library/hide_whats_new
```

### Windows Install

- Download the [Latest Release](https://github.com/tkashkin/Adwaita-for-Steam/releases)
- Ensure you have [Python](#requirements) installed
- Double click the `install_windows` bat script and follow the prompts



### Known Issues

- The Steam window can sometimes appear with just a black background
- The Steam Overlay can be very laggy when downloading something (idk why)
