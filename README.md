# Certificate generation from CSV

This repo contains the latex file that helps to generate participation certificates (for Hackathon organized by Madurai Tech community)  by reading participants data from CSV file.

* `XeLatex` compiler is needed to run the TeX file as `fontspec` package is used to include additional fonts.
* Fonts folder contains the additional font files necessary for the certificates (other than those present in Latex packages). It is invoked using the `\setmainfont` command.
* Background file is loaded using `wallpaper` package and `\TileWallPaper` command.
* Using `datatool` package, CSV data is loaded using `\DTLloaddb` command and column placeholders are created using `\DTLforeach` command. 
* Line spacing is set using `setspace` packages' `spacing` environment. 
* Vertical alignment and center alignment is performed using `\vspace` command and `center` environment. 