# Project: Console Color Sets

This project explores an idea for easily working with color sets
on an ANSI console.  This utility is written in BASH, and it builds
off of work in [bash_patterns][1], using **cocolors** and **keypress**
scripts therein.

## Motivation

When I setup a new computer to which I plan to connect using SSH,
I generally hate the default colors used in several contexts.  The
specific contexts that come to mind are:

- **_ls_**  
  The directory color is usually a dark blue that is very difficult
  to read against dark/black background.  The color sets are defined
  by the environment variable **LS_COLORS**.

- **_man_ pages**  
  The default output of **man** is simple black-and-white, and colors
  greatly improves the experience of reading **man** pages.  **man**
  usually uses **less** as the *pager* program, and **less** colors
  can be set through the set of *LESS_TERMCAP_xx* environment variables.

- **_Emacs_**  
  This is my primary editor, and the color scheme is very important
  to me.  **Emacs** supports *themes* for setting colors wholesale,
  which makes it easier to find coherent colors sets, but changing
  individual colors is time-consuming.  This is the context in which
  I think a color set editing interface would be most useful, but it
  is also the most challenging context to actually implement this idea.

  This is a more difficult challenge, and [there is a dicussion][2]
  of issues around Emacs syntax and other coloring.
  
## Goal

For each context, I'd like to provide the following features:

- The ability to load a set of colors

- An interface that allows a user to select and edit a color target

- Integrate a color-set preview to allow the user to judge how the
  whole set of colors work together.

- An ability to create output that can set a context's color set
  upon opening a console to the computer.



[1]: <http://github.com/cjungmann/bash_patterns.git>   "bash_patterns"
[2]: <README_emacs.md>                                 "Emacs discussion"