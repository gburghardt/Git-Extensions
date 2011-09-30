Installation
============

1. Open a command line shell
2. mkdir ~/bin
3. cd ~/bin
4. git://github.com/gburghardt/Git-Extensions.git ge
5. cd ge
6. chmod +x * (only if the files aren't executable to begin with)
7. Open your bash profile, which could be any of these files: ~/.bash_profile, ~/.bashrc, ~/.profile
8. Add this line and save the file
	export PATH="$PATH:$HOME/bin"
9. Reopen any open shells
10. Type "which ge" from the command line. It should find the ge command.
11. Type "ge help" for a list of commands.