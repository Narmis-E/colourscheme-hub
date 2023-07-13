# colourscheme-hub

This repository serves as a centralized hub for discovering and showcasing various GTK colorschemes. Colorschemes are widely used in modern UNIX customization to alter the colors of applications. Whether you're new to ricing or an experienced ricer looking for something new, this repository offers a collection of GTK colorschemes that have a counterpart for standard terminal 8/16-color ANSI sequences and vice versa.

[I want to add a theme!](#adding-your-theme)


## Popular colourschemes
| Theme                                | Preview                                                   | Widget
| -------------------------------------| --------------------------------------------------------- | ---------------------------------------|
| <p align="center">[arc-dark](https://github.com/Narmis-E/colourscheme-hub/tree/main/arc-dark)</p> | <img src="arc-dark/arc_dark_palette.png" alt="Arc Dark"></img> | <img src="arc-dark/arc_dark_widgets.png" alt="Arc Dark"></img> |
| <p align="center">[catppuccin](https://github.com/Narmis-E/colourscheme-hub/tree/main/catppuccin)</p> | <img src="catppuccin/catppuccin_palette.png" alt="Catppuccin"></img> | <img src="catppuccin/catppuccin_widgets.png" alt="Catppuccin"></img> |
| <p align="center">[dracula](https://github.com/Narmis-E/colourscheme-hub/tree/main/dracula)</p> | <img src="dracula/dracula_palette.png" alt="Dracula"></img> | <img src="dracula/dracula_widgets.png" alt="Dracula"></img> |
| <p align="center">[everforest](https://github.com/Narmis-E/colourscheme-hub/blob/main/everforest/)</p> | <img src="everforest/everforest_palette.png" alt="Everforest"></img> | <img src="everforest/everforest_widgets.png" alt="Everforest"></img> |
| <p align="center">[gruvbox](https://github.com/Narmis-E/colourscheme-hub/blob/main/gruvbox/)</p> | <img src="gruvbox/gruvbox_palette.png" alt="Gruvbox"></img> | <img src="gruvbox/gruvbox_widgets.png" alt="Gruvbox"></img> |
| <p align="center">[material](https://github.com/Narmis-E/colourscheme-hub/tree/main/material)</p> | <img src="material/material_palette.png" alt="Material"></img> | <img src="material/material_widgets.png" alt="Material"></img> |
| <p align="center">[monokai](https://github.com/Narmis-E/colourscheme-hub/tree/main/monokai)</p> | <img src="monokai/monokai_palette.png" alt="Monokai"></img> | <img src="monokai/monokai_widgets.png" alt="Monokai"></img> |
| <p align="center">[nord](https://github.com/Narmis-E/colourscheme-hub/tree/main/nord)</p> | <img src="nord/nord_palette.png" alt="Nord"></img> | <img src="nord/nord_widgets.png" alt="Nord"></img> |
| <p align="center">[onedark](https://github.com/Narmis-E/colourscheme-hub/blob/main/onedark/)</p> | <img src="onedark/onedark_palette.png" alt="One Dark"></img> | <img src="onedark/onedark_widgets.png" alt="One Dark"></img> |
| <p align="center">[rosepine](https://github.com/Narmis-E/colourscheme-hub/blob/main/rosepine/)</p> | <img src="rosepine/rosepine_palette.png" alt="Rosepine"></img> | <img src="rosepine/rosepine_widgets.png" alt="Rosepine"></img> |
| <p align="center">[solarized](https://github.com/Narmis-E/colourscheme-hub/blob/main/solarized/)</p> | <img src="solarized/solarized_palette.png" alt="Solarized"></img> | <img src="solarized/solarized_widgets.png" alt="Solarized"></img> |
| <p align="center">[tokyonight](https://github.com/Narmis-E/colourscheme-hub/blob/main/tokyonight/)</p> | <img src="tokyonight/tokyonight_palette.png" alt="Tokyonight"></img> | <img src="tokyonight/tokyonight_widgets.png" alt="Tokyonight"></img> |

<h2 id="adding-your-theme">Adding your theme!</h2>

If you would like to contribute to repository by adding your own theme, please follow these steps:

1. Clone this repository.
2. Make a copy of the `example` directory with the name of your theme.
3. Your theme directory **must** include a `theme_palette.png`, (if you have a GTK theme) a `theme_widgets.png` and the README.md you copied over.
4. In the README, **replace all instances of "Theme" with your theme name** and **"theme" with your theme name in lowercase** (underscores for spaces).
5. Fill out the rest of the README according to the comments (desc, hex codes, theme source)
6. Commit the changes and push them to your forked repository.
7. Open a pull request to merge your changes.
8. If everything looks good I will merge your theme and add it to the list above.
   
## Theme Image formats
I currently don't have an **absolute** set in stone way for others to reproduce the screenshots, but here are the steps I took:
### theme_palette.png:
Using any termial with your theme applied, run the terminal-colors script from your cloned repo (thanks to [eikenb](https://github.com/eikenb/terminal-colors)) and take a screenshot of the output (zoom in if needed). 
This image **MUST** be cropped to the edges of the colours.\
Make sure `imagemagick` is installed and run the following (replace theme with your theme name in lowercase):
```
convert -scale 528x168 <your cropped colour screenshot> {theme}_palette.png
```
or use gimp.

### theme_widgets.png:
This one may be a little more difficult. Install `lxappearance` and make sure your theme is selected from the list on the left (your theme should be placed in `~/.themes` or `/usr/share/themes`).
Then, shrink the window horizontally until it cannot be shrunk anymore and take a screenshot of the inner window preview:

![](./example_widgets.png)\
e.g here we want to get the cropped preview inside the black borders.\
Save it as {theme}_widgets.png and you should be good to go. It should be near 352x237 but as long as it has a sqaure-ish shape it should look fine.\
If you can't use lxapperance for whatever reason, **please** provide a link to your theme in an issue and I will do it for you.

Again I apologise for not having an absolute method for doing this :/

Happy Ricing!

