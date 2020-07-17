# Kayumi for Windows Terminal

Kayumi is a character from my stories, she represents existential purity. This theme is based on her current favorite colors for Windows Terminal.

This theme will always be open source for those interested in using or contributing to the project.

# Table of Contents
1. [Install](#install)
2. [Activate](#activate)
3. [Recommended Settings](#recommended-settings)

## Install

Start Windows Terminal and click on down arrow symbol from menu bar and select Settings option, or use "*Ctrl + ,*" shortcut.

In your **settings.json** file, find the *schemes* section and paste the content bellow.

```json

"schemes": [
    {
        "name": "Kayumi",

        "background": "#403e41",
        "foreground": "#fcfcfa",

        "black": "#26211E",
        "red": "#C55984",
        "green": "#62BB9E",
        "yellow": "#D78047",
        "blue": "#6292BB",
        "purple": "#8459C5",
        "cyan": "#5E606E",
        "white": "#F7E3CC",

        "brightBlack": "#2E2C2D",
        "brightRed": "#D7708B",
        "brightGreen": "#8DB9A5",
        "brightYellow": "#F9CF9F",
        "brightBlue": "#8DA5B9",
        "brightPurple": "#B36ED6",
        "brightCyan": "#A3A3A3",
        "brightWhite": "#F9F8F1",

        "cursorColor": "#C55984",
        "selectionBackground": "#D7708B"
    }
],

```

## Activate

Now that the color scheme is define, find your profiles section and add Kayumi as your default color scheme or only in one profile.

Example #1: Define as your default color scheme.

```json

"profiles": {
    "defaults": {
      "colorScheme": "Kayumi"
    },
}

```

Example #2: Define the color scheme only in one profile.

```json

{
  "name": "Ubuntu",
  "hidden": false,
  "source": "Windows.Terminal.Wsl",
},

```

## Recommended Settings

Athough this part is optional, for having the best results I recommend using as default profile, using opacity 0.96 and the Fira Code, 14pt font.

```json
"defaults":
{
    // Put settings here that you want to apply to all profiles.
    "acrylicOpacity": 0.96,
    "colorScheme": "Kayumi",
    "fontFace": "Fira Code",
    "fontSize": 14,
    "useAcrylic": true
},
```

Configuring your **ZSH** with Spaceship Prompt Theme will also help the look in WSL profile.

```zsh

ZSH_THEME="spaceship"

SPACESHIP_PROMPT_ORDER=(
  user          # Username section
  dir           # Current directory section
  host          # Hostname section
  git           # Git section (git_branch + git_status)
  hg            # Mercurial section (hg_branch  + hg_status)
  exec_time     # Execution time
  line_sep      # Line break
  vi_mode       # Vi-mode indicator
  jobs          # Background jobs indicator
  exit_code     # Exit code section
  char          # Prompt character
)
SPACESHIP_USER_SHOW=always
SPACESHIP_PROMPT_SEPARATE_LINE=false
SPACESHIP_PROMPT_ADD_NEWLINE=false
SPACESHIP_CHAR_SYMBOL="λ"
SPACESHIP_CHAR_SUFFIX=" "

```

That's all, happy coding! :heart:
