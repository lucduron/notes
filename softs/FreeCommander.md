FreeCommander
=============

Brief: freeware (personal or professional use) alternative to the standard windows file manager

# Integrate Cygwin console (ie replace cmd.exe by mintty.exe):
Settings > DOS box command specification:
`C:\cygwin\bin\mintty.exe -i /Cygwin-Terminal.ico /bin/env CHERE_INVOKING=1 /bin/bash --login`

Source: https://gist.github.com/b6a396f543facc7a01cf.git

# Configure Emacs GUI (emacs-w32) as file editor
Settings > Programs > Editors (fields 'Program' and 'Parameter' are separated below by two whitespaces)
* directly: `C:\cygwin\bin\emacs-w32.exe  %ActivSel%`
* with run.exe: `C:\cygwin\bin\run.exe  /usr/bin/emacs-w32 %ActivSel%` (no background dos window, but path contains whitespace(s))

## Invoke Emacs (emacs-w32) from Cygwin
Problem: FreeCommander is using windows path and emacs cygwin path styles... Two solutions:
* add package windows-path in emacs
* use a script (e.g. python, bash), but is slower

/!\ Take care of whitespaces in path
