# RubyMine URL Handler

This package contains a launcher to open files in RubyMine at the defined line
number and an associated desktop file that conforms to the Desktop Entry
Specification for use in Gnome and KDE desktop environments.

## Installation

    cp rubymine-url-handler /usr/bin/rubymine-url-handler
    desktop-file-install rubymine-url-handler.desktop

## Usage

It can be used to open files at the specified line from within the browser by 
placing a link of the following kind in the markup:

    print "<a href="x-mine://open?file=$file&line=$line">Open with RubyMine</a>";

## Commandline usage

    FILE="/path/to/filename.rb"
    LINE=35
    ./rubymine-url-handler "x-mine://open?file=${FILE}&line=${LINE}"

This script is used in the ARCH linux package to be found at  
rubymine-url-handler https://aur.archlinux.org/packages/rubymine-url-handler/

## License

GNU GENERAL PUBLIC LICENSE
