What is it?
-----------
MultiTail allows you to monitor logfiles and command output in multiple windows in a terminal, colorize, filter and merge. http://vanheusden.com/multitail/

Check [http://vanheusden.com/multitail/](https://vanheusden.com/multitail/screenshots.html) for screenshots and more info.


Help?
-----
For help at any time, press F1.


How to compile
--------------
By default multitail requires the ncursesw library (ncursesW!) to compile and run.
You can choose to use the non-wide char version (ncurses) by setting UTF8_SUPPORT to "no"
in the makefile. Note that this disables UTF8 support.
On Cygwin, you need the libpcre-devel package.


Tips
----
You can also use MultiTail to view logfiles on other hosts!
How?
Like this:
multitail -l "ssh username@host tail -f file"
Q: but then I cannot enter the password!
A1: use authentication via keys
A2: or use "ssh-agent": then you only once have to enter your passphrase (so login once
    to that host manually, and then start MultiTail)


Q & A
-----
Q: the program fails then resizing the terminal-window
A: solution: upgrade ncursesw to version 5.3 (or more recent)

Q: when I use the -l option on some program, I get nothing in the window
A: now that is strange! please tell me what program you're trying to interface to MultiTail.
   please do: any help is appreciated!


License
-------
See the LICENSE file.


For fixes, updates and tweaks please send a PR via github.
