## About
As part of the Machine Learning Module from the [DAS Data Science](https://weiterbildung.zhaw.ch/de/school-of-engineering/programm/das-data-science.html) education at [ZHAW](https://www.zhaw.ch), I wrote a summary paper in german about ["A Critical Review of Recurrent Neural Networks for Sequence Learning"](http://arxiv.org/abs/1506.00019) (Lipton, Berkowitz, Elkan).

## Dependencies
* pandoc
* TeX distribution (only for PDF)
* bibtex file (generated with Zotero)
* Sublime Text 3 (ST3)
  * Markdown Extended
  * CiteBibtex
  * Pandoc

## Hints
in SublimeText 3:
* `F10` shows the entries from the bibtex.bib
* "CiteBibtex: extract citations in current file" -> extracts the used citations and stores them in a local bibex file
* "Pandoc" -> "PDF" creates the PDF file from the markdown file

on the command line run the following command to create the PDF document from the markdown file:
```
pandoc writing_assignment_machine_learning.markdown --latex-engine=xelatex --filter pandoc-citeproc \
 -o rnn_writing_assignment.pdf
```
