- Prerequisite:
	- {{embed [[How to Install Flatpak and Setup Flathub]]}}
- install [flatpak] yazi
	- #+BEGIN_QUOTE
	  flatpak install flathub io.github.sxyazi.yazi
	  #+END_QUOTE
- create [optional] shell function
	- For a more convenient way to launch Yazi by simply typing `yazi`, you can add a shell function to your shell's configuration file.
	- add the following line to preferred shell configuration file
		- #+BEGIN_NOTE
		  CLI Interpreter: *Bash*
		  Config file: *~/.bashrc*
		  #+END_NOTE
		- #+BEGIN_QUOTE
		  function yazi() {
		    flatpak run --command=yazi io.github.sxyazi.yazi "$@"
		  }
		  #+END_QUOTE
	- reload shell
		- #+BEGIN_QUOTE
		  source ~/.bashrc
		  #+END_QUOTE