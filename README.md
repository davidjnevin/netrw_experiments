# Netrw Experiments

A sandbox to learn and experiemnt with vim netrw.

This repo contains simple folder strucutres with files.

## Commands in Netrw

`D` create directory

`cd<cr>` make current directory the working directory

`%` create new buffer, must be saved to write.

:Lexplore open the file explorer on the left side in a window.

`<ctrl>w+h/j/kl` switch to other window.

`i` change the listing style. Cycle through thin, long, wide or tree. (g:netrw_liststyle=0-3)

`a` toggle show hidden file, show all or only show hidden files. Hidden files are defined using comma seperated regex patterns. (g:netrw_list_hide= '\(^\|\s\s\)\zs\.\S\+') Hide .files

`R` rename a file or directory

## Moving files

	From the netwr help files:
    **WARNING**: moving files is more dangerous than copying them.
	A file being moved is first copied and then deleted; if the
	copy operation fails and the delete succeeds, you will lose
	the file.  Either try things out with unimportant files
	first or do the copy and then delete yourself using mc and D.
	Use at your own risk!

Process:

`mt` mark the target folder
`mf` mark the file
`mm` make the move

`mF` unmark all files in the current directory
`mu` unmark all marked files

## Copying Files

Process

`mt` mark the target folder
`mf` mark the file
`mc` make the copy

