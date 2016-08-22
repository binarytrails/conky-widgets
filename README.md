# Conky-widgets

> Conky is a system monitor that renders text on desktop or to own transparent window. Command line options will override configurations defined in config file.

The purpose is to revive and adapt the various artist works to my personal sense of aesthetics.

# Install

These are made for Conky 1.9.0 with lua support.

    mkdir -p ~/.conky
    git clone https://github.com/sevaivanov/conky-widgets ./conky/widgets

# Exploring

I will mainly use these but there are more:

	$ conky -h
	Usage: conky [OPTION]...
	   ...
       -q, --quiet               quiet mode
	   -D, --debug               increase debugging output, ie. -DD for more debugging
	   -d, --daemonize           daemonize, fork to background
	   -x X                      x position
	   -y Y                      y position
	   ...

Then, you can test them with:

    cd ~/
    conky -D -c ~/.conky/widgets/<name>/conkyrc

# Starting on login

You can put the below command in ```~/.xprofile``` file.

    conky -qd -x -1000 -y 1000 -c ~/.conky/widgets/<name>/conkyrc

It will put your widget on the top right screen corner.

You need one conky command per widget.

# License

It's either the ones they have or these:

The code is licensed under a GNU General Public License [GPLv3](http://www.gnu.org/licenses/gpl.html).

The contents and design are licensed under a Creative Commons Attribution-ShareAlike 3.0 Unported License.

![https://i.creativecommons.org/l/by-sa/4.0/88x31.png](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)
