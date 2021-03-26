# How to Install LaTeX

This is a guide to help you install LaTeX on your personal computer. If you
use a web based editor for LaTeX, this guide isn't for you.

## Full Installations

### Windows

To install LaTeX on Windows, the easiest way to do this is to install [proTeXt](https://tug.org/protext/).
The installation process is pretty straightforward, it's a standard Windows
installer. It will also install A LaTeX editor and a PDF viewer for you as well.

### macOS

#### macTeX

If don't use a package manager, the easiest way to install LaTeX is through [MacTeX](https://www.tug.org/mactex/).
It downloads as a .pkg file (around 4gb in size), and then runs a installer.
If in doubt, say yes to the defaults.

#### homebrew / nix

If you use a package manager on macOS (you will know if you do) LaTeX is
available in all of the major package manager's repositories.

If you use [homebrew](https://brew.sh/) the command to run is:

`brew install mactex`

If you use [nix](https://nixos.org/download.html)

`nix-env -iA nixpkgs.texlive.combined.scheme-full`

### Linux

Typically, LaTeX is offered either in your package manager's repository.

For distros that use `apt`, the (typical) command to run is:

`apt install texlive-full`

### BSD

For all the Major BSD variants (Free, Open, and Net), LaTeX is available in your
ports collection.

## TinyTeX

For those who don't want to have multiple gigabytes of hard drive space eaten up
by a LaTeX installation, [TinyTeX](https://yihui.org/tinytex/) provides a simpler alternative (however it requires using the command line).

Follow the instructions on the website (it involves downloading an installer script,
then running said installer script).

Once TinyTeX is installed, you will want to use `tlmgr` to install the nessecary LaTeX
packages (which are documented in [PACKAGES](./PACKAGES.md))

**NOTE:** This is the method that I personally use, and it works quite well if you are
wanting to save disk space for a little inconvience.

### Windows

Admittedly, this is more difficult than installing TinyTeX on Linux or macOS, but is still
pretty straightforward.

If you have [R](https://www.r-project.org/) installed, you can run the following code in the R repl:

```
install.packages('tinytex')
tinytex::install_tinytex()
```

To Uninstall, run:

```
tinytex::uninstall_tinytex()
```

**NOTE** This method will work for Linux and macOS too

Otherwise, you will need to download the latest zip file from the TinyTeX releases page [here](https://github.com/yihui/tinytex/releases).
And follow the instructions on the TinyTeX website.

### Linux / macOS

If you are using Linux, you can go to the same releases page and download the file that ends in `.tar.gz`.
Save it in the root of your home folder (`/home/yourname`), and run the following:

```
tar xvf downloaded_file.tar.gz
```

For macOS, it's the same procedure, except you will download the `.tgz` file.

## Important Notes

This guide is likely missing some edge case that you may run into. When in doubt, visit the TinyTeX website,
as it has more up to date information, as well as fixes for common problems.
