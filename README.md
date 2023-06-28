# BY8
BY8, or BYE, is a linux commandline tool for kicking out logged in users on your machine. This can be used for kicking out attackers on a host, but it could equally well serve as a tool for closing down an x session (closing the tty) during debugging.

# Installation
```
git clone https://github.com/arch-err/BY8.git
```
## Dependencies
 - fzf

### Arch-based distributions
```
sudo pacman -S fzf
```
### Debian-based distributions
```
sudo apt install fzf
```

# Usage
```
$ ./BY8 -k
*Choose session to kick*
```
OR
```
$ ./BY8 -h
```
OR
```
$ ./BY8 -b 
user1	tty1	xinit	/home/user1/.config/xinitrc
user2	tty2	xinit	/home/user2/.config/xinitrc
user3	pts/8	-bash	

What should be grepped for to identify the target? Could be a username, terminal-type, etc.
I understand regex (PCRE) btw, so feel free to use your big brain.
 > *Input identifier*
```


