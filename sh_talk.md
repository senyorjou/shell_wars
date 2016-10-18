##Shell Talk

- ##### History
    - Man talks to machine, _hello hardware give me this file please_
    - 1971: Thompson Shell
    - 1977: Bourne Shell
        - System V, AIX, HP-UX, SCO, Solaris
    - 1978: C shell
        - BSD
    - 1983: Korn Shell
    - 1989: Bourne Again shell (bash)
        - POSIX
        - Linux, Mac
    - 1990: Z shell

- ##### What's that "home of a turtle"?
	- Terminal, shell, tty, console -> WTF!
	- terminal = tty: input/output environment
   	- console: physical terminal connected to computer
   	- shell: command line interpreter.
   	- terminal emulators or pseudo terminals
        - Things get even more complicated when you start running pseudo terminals inside pseudo terminals, à la screen(1) or ssh(1).

- ##### Overview bash basic concepts
    - Primary interface that users see when they log in, whose primary purpose is to start other programs.
    - man bash
    - Shell builtin few known commands: pwd, cd, echo, history, kill
    - Expansion. __WRITE FEW SUPER USEFUL EXAMPLES__
        - Pathname expansion
        - Tilde expansion
        - Arithmetic expansion
        - Brace expansion
        - Parameter expansion: Environment variables
        - Command Substitution
        - Quoting
    - I/O Redirection: Output, Input, pipelines. __WRITE FEW SUPER USEFUL EXAMPLES__
        - example pipelines: filter and word count freq __WRITE ONE USEFUL EXAMPLE__
    - Job Control
        - ps, kill (signalling), jobs, fg, bg
    - History
    - Readline Functions binding. ```bind -P```
    - Configuration (distribution dependent)
        - /etc/profile
            The systemwide initialization file, executed for login shells
        - /etc/bash.bashrc
            The systemwide per-interactive-shell startup file
        - ~/.bash_profile
            The personal initialization file, executed for login shells
        - ~/.bashrc
            The individual per-interactive-shell startup file
        - ~/.inputrc
            Individual readline initialization file


- ##### Bash VS Zsh. Main differences
    - Software License
        - Bash: GNU, GPL
        - Zsh: MIT-like
    - Compatibility/Portability
        - Bash: POSIX.2: Shell and Utilities (IEEE Std 1003.2-1992)
        - Zsh: Enhanced features not following POSIX

- ##### Oh my zsh. Da hipster shell
    - Programmable command-line completion that can help the user type both options and arguments for most used commands, with out-of-the-box support for several hundred commands
    - Sharing of command history among all running shells
    - Extended file globbing allows file specification without needing to run an external program such as find
    - Improved variable/array handling
    - Editing of multi-line commands in a single buffer
    - Spelling correction
    - Various compatibility modes, e.g. zsh can pretend to be a Bourne shell when run as /bin/sh
    - Themeable prompts, including the ability to put prompt information on the right side of the screen and have it auto-hide when typing a long command
    - Loadable modules, providing among other things: full TCP and Unix domain socket controls, an FTP client, and extended math functions.
    - The built-in where command. Works like the which command but shows all locations of the target command in the directories specified in $PATH rather than only the one that will be used.
    - Named directories. This allows the user to set up shortcuts such as ~mydir, which then behave the way ~ and ~user do.
    - Themes and plugins
