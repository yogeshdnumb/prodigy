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

_just download the script and add it to path (optionally the config file at ~/.config/prodigy/prodigy.conf)_

```bash
wget https://github.com/yogeshdcool/prodigy/raw/main/prodigy -P ~/.local/share/bin # or anywhere at path
# optional if ot it prodigy uses dekstop files
mkdir -P .config/prodigy
wget -O prodigy.conf https://github.com/yogeshdcool/prodigy/raw/main/prodigy.conf -P ~/.config/prodigy
```

## Configuration

````
text=alacritty -e nvim

image=nsxiv # by general mime type ("IMAGE"/jpege)
jpeg=nsxiv  # by specific mimetype (image/"JPEG")
jpg=nsiv    # by extension (wallpaper."jpg")

https=librewolf
x_scheme_handler=librewolf # all urls (not x-scheme-handler...use _ not - )
directory=thunar

terminal=alacritty # for opening files using desktop files
launcher="rofi -dmenu -p open-with"



```alcitty -e bin

**for mimetypes use \_ instead of - **

## Contributing

Contributions are always welcome!
_please critisize me ;)_

## Authors

-   [@yogeshdcool](https://www.github.com/yogeshdcool)

## License

[MIT](https://choosealicense.com/licenses/mit/)
````
