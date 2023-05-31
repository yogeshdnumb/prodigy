# Prodigy

**A simple yet powerful alternative to xdg-open**

Automatically opens a file or url by suitable application

![Shell Script](https://img.shields.io/badge/shell_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

## Features

-   Easy configuration
-   Quite intelligent (_not really lol_)
-   Supports terminal and launcher

### Supports opening file by

-   Extension
-   MimeType
-   Desktop files
-   Asks you if no applications found

## Installation

_just downlaod the script and add it to path (optionally the config file at ~/.config/prodigy/prodigy.conf)_

```bash
wget https://github.com/yogeshdcool/prodigy/raw/main/prodigy -P ~/.local/share/bin # or anywhere at path
# optional
mkdir -P .config/prodigy
wget -O prodigy.conf https://github.com/yogeshdcool/prodigy/raw/main/prodigy.conf.example -P ~/.config/prodigy
```

## Configuration

```
terminal=alacritty     --> terminal for needed applications (= is used for options)
launcher=rofi -d       --> launcher to use if no applications found

mp3:       vlc          --> by Extension (: is used)
audio/mp3: vlc           --> by mimetype
audio/:    vlc          --> by the first part of mime type (general mime)

x-scheme-handler/https: librewolf        --> supports urls
application/x-bittorent: deluge
```

## Contributing

Contributions are always welcome!  
_please critisize me ;)_

## Authors

-   [@yogeshdcool](https://www.github.com/yogeshdcool)

## License

[MIT](https://choosealicense.com/licenses/mit/)
