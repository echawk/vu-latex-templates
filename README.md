# LaTeX Templates for VU students

This repository contains templates for various paper formats that are used at Valparaiso University.
One notable exclusion from all of these template files is the addition of the honor code at the end of the document.

## How to compile

Generally, all you need to run is the following:

```
pdflatex <file>.tex
biber <file>
pdflatex <file>.tex
```

That will compile your document, and add in citations.

If you don't need bibliography support, you can just run:
`pdflatex <file>.tex` and be set.
