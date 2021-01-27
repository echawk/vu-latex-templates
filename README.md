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

* If you don't need bibliography support, you can just run: `pdflatex <file>.tex` and be set.

## Which Template?

Usually your Professor will tell you which paper format s/he will expect. But in the event that they *don't* tell you, here are some examples:

| Class Type     | Formatting Style | Citation Style |
| :------:       | :--------:       | :------:       |
| Christ College | Chicago          | Chicago        |
| Heath Science  | APA7             | APA            |
| Psychology     | APA7             | APA            |
| Valpo Core     | MLA              | MLA            |

## I need to see an example...

All of the example documents are under `examples/`, and should hopefully illustrate how to to
do all of the things you need to do in word, in LaTeX.
