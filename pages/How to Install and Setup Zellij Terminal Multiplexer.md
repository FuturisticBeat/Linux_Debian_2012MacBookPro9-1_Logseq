- download latest github release for x86_64
	- #+BEGIN_QUOTE
	  wget [https://github.com/zellij-org/zellij/releases/latest/download/zellij-x86_64-unknown-linux-musl.tar.gz](wget https://github.com/zellij-org/zellij/releases/latest/download/zellij-x86_64-unknown-linux-musl.tar.gz)
	  #+END_QUOTE
- extract the tarball
	- #+BEGIN_QUOTE
	  tar -xvf zellij-x86_64-unknown-linux-musl.tar.gz
	  #+END_QUOTE
- move extracted zellij directory of files to /usr/local/bin
	- #+BEGIN_QUOTE
	  sudo mv zellij /usr/local/bin
	  #+END_QUOTE
- setup preferred starting layout
	- see [documentation](https://zellij.dev/documentation/layouts.html)
- setup preferred font -> JetBrainsMono Nerd Font
	- {{embed [[How to Install Custom System Fonts]]}}
- create [optional] keyboard shortcut
	- launch preferred terminal emulator with zellij in preferred layout