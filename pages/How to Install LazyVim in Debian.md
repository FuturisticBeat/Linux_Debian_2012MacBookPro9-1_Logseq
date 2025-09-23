- #+BEGIN_NOTE
  requires a recent version of neovim (version 0.11.2 or higher)
  #+END_NOTE
- install recent version of neovim using AppImage from Github
	- #+BEGIN_QUOTE
	  curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.appimage
	  #+END_QUOTE
- make downloaded AppImage executable for local user
	- #+BEGIN_QUOTE
	  chmod u+x nvim-linux-x86_64.appimage
	  #+END_QUOTE
- move executable to /usr/local/bin for global use in CLI
	- #+BEGIN_QUOTE
	  sudo mv nvim.appimage /usr/local/bin/nvim
	  #+END_QUOTE
- create [optional] backup of existing neovim configs
	- #+BEGIN_QUOTE
	  mv ~/.config/nvim ~/.config/nvim.bak
	  mv ~/.local/share/nvim ~/.local/share/nvim.bak
	  mv ~/.local/state/nvim ~/.local/state/nvim.bak
	  mv ~/.cache/nvim ~/.cache/nvim.bak
	  #+END_QUOTE
- clone [git] starter LazyVim config into ~/.config/nvim
	- #+BEGIN_QUOTE
	  git clone https://github.com/LazyVim/starter ~/.config/nvim
	  #+END_QUOTE
- remove cloned .git folder (starter configs will be customized and version controlled by local user)
	- #+BEGIN_QUOTE
	  rm -rf ~/.config/nvim/.git
	  #+END_QUOTE
- install [apt] tree-sitter-cli (tree-sitter parser manager)
	- #+BEGIN_NOTE
	  [*required dependency*]
	  when this is not installed there will be errors displayed on nvim load
	  #+END_NOTE
	- #+BEGIN_QUOTE
	  sudo apt update
	  #+END_QUOTE
	- #+BEGIN_QUOTE
	  sudo apt install tree-sitter-cli
	  #+END_QUOTE