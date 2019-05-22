# Lecture Notes
This is my collection of lecture notes (+ other study things) for courses that I've taken during my undergraduate studies at the University of Alberta.

Most (if not all) of them are typeset to look like a Dungeon and Dragon guide book. **Why?** Well the short story is that I was bored in my Operating Systems Lab and experimented with different LaTeX templates to see which ones I liked. I choose this template: [DND-5e-LaTeX-Template](https://github.com/rpgtex/DND-5e-LaTeX-Template). The rest is history I guess.

This collection is a subset of my School-Notes repository which are my personal notes kept private as it contains active assignments, copyright assets, experimental LaTeX code, or other forbidden knowledge of the arcane arts :stuck_out_tongue_winking_eye:.    

## (Full story) Why the DnD template?
In the beginning of the Winter 2019 semester I decided to LaTeX all my notes. I had some experience in the previous semesters doing some of my assignments in LaTeX and have found the finished work amazing. So why not LaTeX all my notes, it would look amazing at the end. Moreover, I wanted to try out a new studying technique where I would either write or type my notes in class and typeset them after as review so I can understand the content better. All I needed was a template so I can typeset my notes without worrying about the style and formatting of the notes, what LaTeX was design for. 

Now this template was chosen by accident. I discovered this template during a lab session for CMPUT-379 and as a joke typeset my MATH-115 notes with it. It turns out, the different boxes used in the template was great at showing important theorems, definitions, notes, etc. The die tables used for DnD was great at describing different variables within an equation or formula.

In addition, I started playing DnD after a 4 month hiatus and the DM finds it hilarious that I decided to typeset my notes to look like a Dungeons and Dragon book. 

## Courses
Some are incomplete, for example courses that I've taken during the Fall of 2018 are incomplete as this was before I decided to LaTeX all my notes, only my assignments.

| Course ID | Instructor        | Term        |
| :-------- | :---------------- | :---------- |
| MATH-2000 | Jeff Bleaney      | Spring 2017 |
| MATH-1410 | Habiba Kadiri     | Fall 2017   |
| CMPUT-291 | Davood Rafiei     | Fall 2018   |
| ECON-299  | Alexander Gainer  | Fall 2018   |
| MATH-115  | Mohammad Niksirat | Winter 2019 |
| ECON-282  | Andrew Wong       | Winter 2019 |
| EAS-212   | Paul Myers        | Winter 2019 |
| CMPUT-496 | Martin Muller     | Winter 2019 |
| CMPUT-379 | Ioanis Nikolaidis | Winter 2019 |
| CMPUT-415 | J Nelson Amaral   | Fall 2020   |

## The "Wacky" Cover Art
As a Computing Science major I get exposed to a lot different programming and computing books. For example:
- Compilers: Principles, Techniques, and Tools used in compiler design classes is affectionately known as the **Dragon Book**
- Operating System Concepts by Silberschatz, Galvin and Gagne is often called the **Dinosaur Book**
- Structure and Interpretation of Computer Programs is often called the **Wizard Book**
- Database System Concepts is sometimes called the **Sailboat Book**
- Introduction to Automata Theory, Languages, and Computation, among experts is known as the **Cinderella Book**
- Lions' Commentary on UNIX 6th Edition, with Source Code, commonly referred to as the **Lions Book**
- Mastering Regular Expressions is called the **Owl Book**

A lot of it can be traced back to O'Reilly Media as they started this trend as a way to distinguish themselves from other publishers.

To continue the trend I decided to give a fantasy flair to further increase the DnDness of my notes. Plus they provide a good metaphor to the content of the course. 

I'm half tempted to call CMPUT-415 which is the compiler design course "How to Clang Your Dragon" 

## To Build my Notes
In order to build these notes yourself you need at least one program:
- LaTeX typesetting engine: Either TeX Live (full) or MikTeX is fine, TeX Live is preferred.
- Rubber (you can manually build the notes yourself but its more of a pain) (recommended)
- GNU Make (recommended) if you want to use the Makefile.

Goto the root directory that contains the Makefile and type
``` make 
make full       # Build with the full paper background
make print      # Make the druids happy by building the notes with a white paper background 
make clean      # Clean the aux files
```
To build it manually use this command
```
pdflatex -synctex=1 -interaction=nonstopmode filename.tex 
# You may need to recompile as latex needs multiple passes in order to get cross-references to work. 
```

## Future Goals
- Typeset mp4s or gifs into the notes. (I know this is possible within Windows Adobe Acrobat but not on Linux Adobe Acrobat)
- Create a .sty template for assignments (Not in DnD format, Summer 2019 project)

## Done/Somewhat Done
- Easily change the color of the boxes within the same document. (Beta)
- Create a collections of snippets, macros and templates so it is easier to typeset my notes (Beta)
- Speed up the compiling process. (Beta)
- Quickly create and typeset images (Alpha)

## Disclaimer
These notes are not official, nor are they endorsed by the instructor, Wizard of the Coast, Games Workshop or any other company unless explicated stated. Moreover, these notes haven't been proofread by the instructor (with a few exceptions). Therefore, they are liable to errors or typos. If you find such an error, I'd be greatly appreciate it if you could open a pull request (if you are proficient with LaTeX and have the required template) or open an issue (so that I can fix it). 

## Copyright
Due to the fact that I am using assets from the instructor as well images from Wizard of the Coast and/or other companies' IPs. If requested by their rightful owners I may have to remove them from the repository. For some notes I will only provide the complete PDFs and not the LaTeX code if it requires access to certain copyright assets. 


