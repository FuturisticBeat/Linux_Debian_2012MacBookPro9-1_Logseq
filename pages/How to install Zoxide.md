- install [apt] zoxide
	- #+BEGIN_QUOTE
	  sudo apt update
	  #+END_QUOTE
	- #+BEGIN_QUOTE
	  sudo apt install zoxide
	  #+END_QUOTE
- add the following line to preferred shell configuration file
	- #+BEGIN_NOTE
	  CLI Interpreter: *Bash*
	  Config file: *~/.bashrc*
	  #+END_NOTE
	- #+BEGIN_QUOTE
	  eval "$(zoxide init bash)"
	  #+END_QUOTE
- reload shell
	- #+BEGIN_QUOTE
	  source ~/.bashrc
	  #+END_QUOTE