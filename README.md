# frequentlyuseddnfcommands
These are some of my frequently used Fedora package management commands.

## List all repository

    dnf repolist

## List all packages in a repository

    sudo dnf repository-packages repo-name list

## List all packages installed from a repository

    sudo dnf repo-pkgs repo-name list installed
	
## List installed packages

	sudo dnf list installed
	sudo dnf list installed | grep -ie package-name

## DNF history commands

    sudo dnf history
    sudo dnf history info #
    sudo dnf history undo last
    sudo dnf history redo #
	
## Import signing key

    sudo rpm --import package-signing-key.pub

## Downgreade a pacakge

    sudo dnf --allowerasing downgrade package-name

## How to terminate a frozen ssh connection.

	$ Enter
	$ ~
	$ .
	
[Properly close a frozen SSH session](https://infertux.com/posts/2012/12/20/properly-close-a-frozen-ssh-session/)

## Convert a webm file to gif

    ffmpeg -i input.webm -pix_fmt rgb24 output.gif

[How to do I convert an webm (video) to a (animated) gif on the command line?](https://askubuntu.com/a/506672/106123)


## Delete history

    history -c #clear all history
	history -d lineNumbe # clear the history lineNumber item

## Restart kwin

    kwin_x11 --replace &
	
## Restart Plasmashell

    killall -s SIGSEGV plasmashell

## Mount Android devices using simple-mtpfs

	simple-mtpfs mountpoint [options]
	simple-mtpfs --device <number> mountpoint [options]
	simple-mtpfs --list-devices
	fusermount -u mountpoint

## Resize Images

	mogrify -resize 1222x2444 -quality 100 -path /path/to/converted *.png # maintains aspect ratio
	mogrify -resize 800x1094! *jpg #doesn't maintain aspect ratio
	
