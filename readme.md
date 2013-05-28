# SASS functions

An automated SASS base64 inline image generator

## Installation

```bash
sudo gem install sass
sudo gem install smusher
```

## Starting SASS from the command line

When starting SASS from the command line, be sure to invoke the url64 module:

```bash
sass --watch sass:css -r ./sass/functions/sass-functions.rb
```

## Usage

Accepts a variety of formats (GIF/JPG/PNG/SVG), in any CSS declaration. Use `url64` anywhere you'd use a plain old `url`. For example:

```sass
background-image: url64("../images/image.png")
```

NB: Be sure to use quotes around your URL, otherwise SASS will throw an error.

`rand` accepts a max number:

```sass
font-size: ( 10 + rand(5) )+px
```
