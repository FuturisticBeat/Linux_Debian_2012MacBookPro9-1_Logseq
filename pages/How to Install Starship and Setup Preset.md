- install [apt] starship
	- #+BEGIN_QUOTE
	  sudo apt update
	  #+END_QUOTE
	- #+BEGIN_QUOTE
	  sudo apt install starship
	  #+END_QUOTE
- setup shell to initialize starship
	- #+BEGIN_NOTE
	  Bash is the shell used in this guide
	  #+END_NOTE
	- add the following line at the end of ~/.bashrc to initialize starship on shell start
		- #+BEGIN_QUOTE
		  echo "$(eval starship init bash)" >> ~/.bashrc
		  #+END_QUOTE
- install a Nerd font and set it as terminal font
	- #+BEGIN_NOTE
	  this is a prerequisite to using starship presets
	  #+END_NOTE
		- {{embed [[How to Install Custom System Fonts]]}}
- configure starship config using an existing from [https://starship.rs/presets](https://starship.rs/presets)
	- e.g.
		- #+BEGIN_QUOTE
		  starship preset catppuccin-powerline -o ~/.config/starship.toml
		  #+END_QUOTE
- see: [official installation guide](https://starship.rs/guide/#🚀-installation)
- see: [nerd fonts symbols cheat-sheet](https://www.nerdfonts.com/cheat-sheet)