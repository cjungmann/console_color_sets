# Console Color Sets: Emacs

Return to [README.md](README.md)

In Emacs, an effective syntax-highlighting color scheme can significantly
enhance productivity.  Personally, I find it very tedious to adjust colors
with the Emacs interface, so I am practicing my BASH programming with an
attempt to create an aid for setting Emacs colors.

An effective color scheme should help a user navigate a long, dense text
document, to quickly identify and locate items of interest and to expose
the intention of the author.

As I prepare to create this tool, I would like to compile a list of syntax
classes that are likely to coexist on a page in order to gently prompt
consideration of the syntax classes and to create a sample document that
can quickly show how the colors work together.

## Limitations

### Generating code

My intention is to provide a means for a user of this tool to incorporate
selected colors into their Emacs configuration.  I will not attempt to
edit the `~/.emacs.d/init.el` file, but to generate a script that could
be copied into that file.

### Color specifications only

This is a BASH experiment, and works on a console, so I'm not going to
try to set all font-face attributes because many only pertain to a GUI.
For starters, my intention will be to only support setting foreground
and background colors.

## Resources/Research

The following are resources I am using to compile a list of font faces
that should be considered together when setting up colors:

- [Standard Faces (14.10 in Emacs info)][1]
  Part-way down this page is a partial list of faces that temporarily
  change colors, list for lists, selection highlights, etc.  You want
  to consider these colors when you setup fixed syntax colors

- [Font-lock Faces (23.6.7 in ELisp info)][2]  
  This page lists the basic font-lock variables for which one might want
  to define colors.  This list includes keywords, comments, and function
  names, among others.

- [Useless Whitespace (14.16 in Emacs info)][3]
  I learned about this mode while doing this research, and I think that
  enabling syntax-highlighting for useless space could be helpful, as
  long as the highlighting is subtle.




[1]: <https://www.gnu.org/software/emacs/manual/html_node/emacs/Standard-Faces.html>             "standard faces"
[2]: <https://www.gnu.org/software/emacs/manual/html_node/elisp/Faces-for-Font-Lock.html>                      "font-lock variables"
[3]: <https://www.gnu.org/software/emacs/manual/html_node/emacs/Useless-Whitespace.html>         "useless whitespace"

