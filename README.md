# Scripts to extract Keywords

This script extracts keywords from [the online documentation of GMSH](http://gmsh.info/doc/texinfo/gmsh.html). 
The keywords are located in the [`Syntax Index` table](http://gmsh.info/doc/texinfo/gmsh.html#Syntax-index). The operators and command line are excluded.

To make it work, download the documentation on the same folder of the script, name it `doc.html` and launch the script
```bash
python3 extract_keywords.py
```

The result should be N JSON files (probably 2) that should then be copy/paste  into the language file of the GMSH extension. The split in different files is due to the (too) high number of keywords, leading to a bug (on my computer) 