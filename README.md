Single-cell resolution view of the transcriptional landscape of developing *Drosophila* eye.
===

[Radoslaw Kamil Ejsmont](https://github.com/rejsmont)<sup>1,2,3,✉</sup>, [Grace Houser](https://github.com/Grace-Hoxuser)<sup>1</sup>, Natalia Mora Garcia<sup>1,2</sup>, Sara Fonseca Topp<sup>1</sup>, Natalia Danda<sup>1</sup>, Agnes Wong-Chung<sup>1</sup>, Bassem A. Hassan<sup>1,2,✉</sup>
---

<sup>1</sup> Institut du Cerveau et de la Moelle Epinière (ICM) - Hôpital Pitié-Salpêtrière, Sorbonne Université, Inserm, CNRS, Paris, France

<sup>2</sup> VIB Center for the Biology of Disease, VIB, Leuven, Belgium

<sup>3</sup> Current address: Center for Research and Interdisciplinarity (CRI), Paris, France

<sup>✉</sup> Corresponding authors, e-mail: R.K.E <radoslaw.ejsmont@cri-paris.org>, B.A.H. <bassem.hassan@icm-institute.org>

---
[![DOI](https://zenodo.org/badge/147840131.svg)](https://zenodo.org/badge/latestdoi/147840131)


#### [Abstract](manuscript.md#Abstract)
#### [Introduction](manuscript.md#Introduction)
#### [Results](manuscript.md#Results)
#### [Discussion](manuscript.md#Discussion)
#### [References](manuscript.md#References)
#### [Acknowledgements](manuscript.md#Acknowledgements)
#### [Author contributions](manuscript.md#Author-contributions)
#### [Methods](manuscript.md#Methods)
#### [Supplementary material](manuscript.md#Supplementary-material)

---

The manuscript is written in [pandoc markdown](https://pandoc.org/MANUAL.html#pandocs-markdown). It can be rendered into [GitHub Flavored Markdown](https://github.github.com/gfm/) with the following command:

```
pandoc -F pandoc-crossref -F pandoc-citeproc source.md -t gfm --template templates/default.gfm --wrap=none | sed 's/\!\[\*\*\(.*Figure .\) - \(.*\)\](\(.*\.png\))/§![\1](\3)§§<small>§§**\1 - \2§§<\/small>§§---§/' | tr '§' '\n' > manuscript.md
```

and into a PDF with the following command:

```
cat source.md | sed 's/s*\.png/.pdf/' | pandoc -F pandoc-crossref -F pandoc-citeproc --template templates/default.latex --wrap=none -o manuscript.pdf --pdf-engine=xelatex --from markdown+latex_macro -f markdown
```

Version for reviewing (with numbered lines and larger line spacing) can be generated using the following command:

```
cat source.md | sed 's/s*\.png/.pdf/' | pandoc -F pandoc-crossref -F pandoc-citeproc --template templates/review.latex --wrap=none -o manuscript-review.pdf --pdf-engine=xelatex --from markdown+latex_macro -f markdown
```

---

This is a repository for [HassanLab](https://github.com/HassanLab/) publication from RDN-WDP Project. Image processing software used in this research can be found in [RDN-WDP](https://github.com/rejsmont/rdn-wdp) repository. Data mining and postprocessing scripts can be found in [RDN-WDP-Python](https://github.com/rejsmont/rdn-wdp-python) repository. Raw data is posted in [RDN-WDP-Data](https://github.com/rejsmont/rdn-wdp-data) repository.

We decided to write this paper on GitHub with belief that open science also means transparency in how scientific stories are put together and published.  If you found this project interesting and would like to contribute, or if you found an error or a bug in the text, data or associated software, drop me a line at [radoslaw.ejsmont@icm-institute.org](mailto:radoslaw.ejsmont@icm-institute.org) or create a pull request.

*We hope that our openness and transparency would not be abused #dontscoopus.*

---

The contents of this repository as well as the associated data ([RDN-WDP-Data](https://github.com/rejsmont/rdn-wdp-data)) is released under Creative Commons Attribution 4.0 (CC-BY-4.0) license with restriction on scientific publishing (see below). Software from [RDN-WDP](https://github.com/rejsmont/rdn-wdp), [RDN-WDP-Python](https://github.com/rejsmont/rdn-wdp-python) is licensed under MIT license with restriction on scientific publishing (see below).

### Supplement to the licenses (CC-BY-4.0 / MIT)
This repository and the associated repositories hold scientific writing, data and software, neither published nor peer-reviewed. You are free to use them in your project, however you should **NOT** publish a paper in a scientific journal using our data or software before we publish ours, unless you obtain a permission from us. As the paper from this repository has not yet been peer reviewed, please treat the information published here with caution as it may contain errors and change without notice.

**The above supplement to the licenses will be revoked once our paper is accepted for publication.**
