- example font to install
	- #+BEGIN_EXAMPLE
	  JetBrainsMono Nerd Font
	  #+END_EXAMPLE
- install [apt] unzip and wget if not already installed
	- #+BEGIN_QUOTE
	  sudo apt update
	  #+END_QUOTE
	- #+BEGIN_QUOTE
	  sudo apt install unzip wget
	  #+END_QUOTE
- Create a font directory
	- for local users only
		- #+BEGIN_QUOTE
		  mkdir -p ~/.local/share/fonts
		  #+END_QUOTE
	- system-wide for all users
		- #+BEGIN_QUOTE
		  mkdir -p /usr/local/share/fonts
		  #+END_QUOTE
- download the latest release of JetBrains Mono Nerd Font from GitHub
	- #+BEGIN_QUOTE
	  wget -P /tmp [https://github.com/ryanoasis/nerd-fonts/releases/latest/download/JetBrainsMono.zip](https://github.com/ryanoasis/nerd-fonts/releases/latest/download/JetBrainsMono.zip)
	  #+END_QUOTE
- unzip downloaded archive into created font directory
	- #+BEGIN_QUOTE
	  unzip /tmp/JetBrainsMono.zip -d ~/.local/share/fonts/
	  #+END_QUOTE
- rebuild the font-cache
	- #+BEGIN_QUOTE
	  fc-cache -f -v
	  #+END_QUOTE
- clean up temp zipped fonts archive directory
	- #+BEGIN_QUOTE
	  rm /tmp/JetBrainsMono.zip
	  #+END_QUOTE
- verify fonts were correctly installed
	- #+BEGIN_QUOTE
	  fc-list  | grep 'JetBrainsMono'
	  #+END_QUOTE