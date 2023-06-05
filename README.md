# Prodigy

**A simple yet powerful alternative to xdg-open**

Automatically opens a file or url by suitable application

xdg-open is a tool used to open a file using desktop files  
but it is confusing and not friendly with window managers so that's why I created this script as a simple replacement with added features

![Shell Script](https://img.shields.io/badge/shell_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

## Features

-   Easy configuration
-   Quite intelligent (_not really lol_)
-   Supports terminal and launcher
-   Opens a file using the application that supports most types

### Supports opening file by

-   Extension
-   MimeType
-   Desktop files
-   Asks you if no applications found

## Installation

_download the prodigy script, rename it to xdg-open and add it to path. Install alacritty(terminal) and rofi(launcher menu) or change them in the config_  
**or**

```bash
# if you do not have xdg-open or xdg-utils installed
curl -o /usr/bin https://raw.githubusercontent.com/yogeshdcool/prodigy/main/prodigy # or anywhere at path
# if you have xdg-open in your system
curl -o $(which xdg-open) https://raw.githubusercontent.com/yogeshdcool/prodigy/main/prodigy

```

## Configuration

```
image=nsxiv # by general mime type ("IMAGE"/jpege)
jpeg=nsxiv  # by specific mimetype (image/"JPEG")
jpg=nsiv    # by extension (wallpaper."jpg")

https=librewolf
x_scheme_handler=librewolf # all urls (not x-scheme-handler. use _ not - )

text="alacritty -e nvim"
directory="alacritty -e lf"
zip="file-roller"
audio="mpv --no-audio-display"

terminal=alacritty                  # for opening files using desktop files (default)
launcher="rofi -dmenu -p open-with" # (default)

```

**for mimetypes use \_ instead of - **

## Contributing

Contributions are always welcome!
_please critisize me ;)_

## Authors

-   [@yogeshdcool](https://www.github.com/yogeshdcool)

## License

[MIT](https://choosealicense.com/licenses/mit/)
