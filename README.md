brackets-quick-markup
=====================

Brackets Extension that creates a quick markup mode 

## Overview

This is an Extension for [Brackets](https://github.com/adobe/brackets). 

## Features

This extension is accessed in Brackets using menu Edit > Quick Markup Mode or Ctrl-M.

A minimal bottom panel is displayed to indicate you are in quick markup mode. A "mode"
is required because this extension uses a lot of keyboard shortcuts which conflict with
some Brackets standard shortcuts. All other Brackets commands and editing work as expected.

Quick Markup mode allows fast HTML markup generation as your type similar to what how a
rich text editor works. It was created with text formatting in mind, but could be extended
for any kind of markup. It currently only generates HTML.

Start adding text by pressing Ctrl-P to create a paragraph using a <p> tag.
The tag will be wrapped around the current selection.

As you are typing, pressing Ctrl-Enter closes the current <p> tag and starts a new one.
To convert a <p> tag to a heading, where heading refers to any <h1> through <h6> tag,
press Ctrl-1 through Ctrl-6, respectively. At the end of a heading tag, pressing Ctrl-P
close the heading tag, and then starts a <p> tag, as this is most likely what you'll
want next.

You can also use Ctrl-Enter in the middle of a <p> tag (or any heading)
to split the tag. Pressing Ctrl-Delete at the end of the (inner) text of a <p>
or heading tag joins the tag with the following sibling (if tag is the same).
Pressing Ctrl-Backspace at the start of the (inner) text joins with the previous
tag in a similar manner.

You can select text and apply or remove <strong>, <em>, or <del> tags using shortcuts
listed in list below.

Resulting text is properly indented based on Brackets preferences and
the appropriate line end characters are inserted for the current operating system.

You can switch documents while in quick markup mode.

Shortcuts used to generate markup:

1. **Cmd/Ctrl-Enter** -- Split Tag
1. **Cmd/Ctrl-Delete** -- Join Next Sibling Tag
1. **Cmd/Ctrl-Backspace** -- Join Previous Sibling Tag
1. **Cmd/Ctrl-P** -- <p>
1. **Cmd/Ctrl-1..6** -- <h1>..<h6>
1. **Cmd/Ctrl-B** -- <strong>
1. **Cmd/Ctrl-I** -- <em>
1. **Cmd/Ctrl-D** -- <del>

Use Edit > Quick Markup Mode Help or Ctrl-Shift-M to see a list of all shortcuts used by this extension.

There is a lot more that could be done with this extension.
Let me know what enhancements you would like.

## License

MIT-licensed -- see _main.js_ for details.
