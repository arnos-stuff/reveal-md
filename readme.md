# My first experiment with RevealJS

Just install reveal-md and run it in the folder with the markdown file.

```bash
npm install -g reveal-md
reveal-md slides.md -w
```

## Slides

They're in the `slides.md` file.
The hardest part was to figure out how to make my own theme.  

I used the [reveal.js theme generator](https://hakim.se/reveal-js/theme/) to create a theme,  
but I had to download the [Sass dart implementation](https://sass-lang.com/install) to compile it.

```bash
brew install sass/sass/sass
```

## What if I'm on Windows?

You can get [homebrew](https://brew.sh/) on Windows with [WSL](https://docs.microsoft.com/en-us/windows/wsl/install-win10) or simply 
[install it using scoop](https://scoop.sh/):

```bash
scoop install homebrew
```

Then you can install sass with:

```bash
brew install sass/sass/sass
```

## A small demo of the theme

you can find a half [hacked video here](https://dl.dropboxusercontent.com/s/xc3p7w7e914tn99/chrome_H9vzWyXekQ.mp4) based on a friend's math project.