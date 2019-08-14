# neovim-pdf-manual
A shell script to automate building pdfs of the [Neovim](https://neovim.io/) documentation

## What it does
The script fetches the html version of the user documentation from https://neovim.io/doc/user/ with `wget` and puts it in a directory. When its done downloading it converts the html documents with [pandoc](https://pandoc.org/index.html) using the pdf engine `pdfroff`. 

## Problems
As of now it creates a pdf for every html page. Creating the pages on languages with special characters like [Nvim documentation: arabic](https://neovim.io/doc/user/arabic.html) doesn't fully work on my machine as I don't have all the fonts set up.
