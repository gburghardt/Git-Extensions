Git Extensions (ge)
===================

Git Extensions provides some wrapper shell scripts around Git with intelligent defaults.

Installation
------------

1. Open a command line shell
2. `mkdir ~/bin`
3. `cd ~/bin`
4. `git clone git://github.com/gburghardt/Git-Extensions.git ge`
5. `cd ge`
6. `chmod +x *` (only if the files aren't executable to begin with)
7. Open your bash profile, which could be any of these files: ~/.bash_profile, ~/.bashrc, ~/.profile
8. Add this line and save the file: `export PATH="$PATH:$HOME/bin/ge"`
9. Reopen any open shells
10. Type `which ge` from the command line. It should find the ge command.
11. Type `ge help` for a list of commands.

Easy SVN Imports
----------------

The `ge svn` utility provides easy ways to generate an SVN authors file, plus do the initial import into SVN.

	cd path/to/subversion_repository
	ge svn authors -f template > svn_authors.txt
	cd path/to/git/import
	ge svn import

The `ge svn import` utility steps you through the process of importing an SVN repository into Git. If you want to make things scriptable, you can always pass in flags instead of using the interactive mode:

	ge svn import --authors-file=path/to/authors/file --usename=svn_username <svn url> <destination>
