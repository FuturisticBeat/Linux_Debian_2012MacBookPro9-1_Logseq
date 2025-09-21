- add non-free firmware sources to /etc/apt/sources.list
  #+BEGIN_QUOTE
  deb http://deb.debian.org/debian stable main contrib non-free
  #+END_QUOTE
- install Broadcom b43 WiFi firmware
	- id:: 68cf8aea-c0f6-4fb1-84a4-7d1f541a545f
	  #+BEGIN_QUOTE
	  sudo apt update
	  #+END_QUOTE
	- #+BEGIN_QUOTE
	  sudo apt install firmware-b43-installer
	  #+END_QUOTE
- reload installed Broadcom b43 WiFi firmware
	- #+BEGIN_QUOTE
	  sudo modprobe -r b43
	  #+END_QUOTE
	- #+BEGIN_QUOTE
	  sudo modprobe b43
	  #+END_QUOTE