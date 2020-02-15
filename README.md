# Android Font Patcher
Font patcher script by nongthaihoang @ xda

Patch custom fonts to be used on Android.

## Prerequisites
- Linux
- Fontforge

## Usage
- Rename your fonts to match styles with Roboto:

  Thin | ThinItalic | Light | LightItalic | Regular | Italic

  Medium | MediumItalic | Bold | BoldItalic | Black | BlackItalic
- Run command:
  ```
  ./font-patcher [-cn] [FONT]...
  
      -cn  use Roboto Condensed
  ```
  Example:
  
  `./font-patcher Lato-Regular.ttf`
  
  `./font-patcher Inter-Regular.otf Lato-Bold.ttf`
  
  `./font-patcher Lato/Lato-Regular.ttf`
  
  `./font-patcher Lato/Lato-*`
  
  `./font-patcher -cn "Barlow Condensed Regular.ttf"`
  
  For Windows:
  
  `fontforge.exe -script fontpatcher.pe [Roboto] [Your font] ""`
- The generated fonts will be named after Roboto and placed in the same folder as your fonts.
