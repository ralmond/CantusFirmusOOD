# CantusFirumusOOD
Generates a daily cantus firmus for people wanting inspiration for counterpoint.

The goal is to create a web app that randomly selects a cantus firmus from a file, translates it into PDF, MusicXML, and MIDI formats and inserts it into a web template.  

The basic design is as follows.  

The file `cantusfirmi.dat` contains the cantus firmi in a form that is compatable with the `forturne` program.

Each entry looks like:
```
Name [length] (source): music in Lilypond notation
%
```

A blank line with a `%` character is used to mark the entries.  The length and the source are optional.

The main program would:
1) Select a random entry from `cantusfirmi.dat`.
2) Convert it to PDF, MusicXML and MIDIformats
3) Produce a web page bundle with those supporting files and a template XHTML file linking them.

The XHTML and bundle could then be included in a web page.

Contributers welcome.

