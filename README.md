# Resume [![resume](https://img.shields.io/badge/example-pdf-green.svg)]()

This is my resume - a heavily modified fork of [awesome-cv](https://github.com/posquit0/Awesome-CV). Feel free to use for your own job-hunting needs as you see fit!

## Setup

I recommend downloading the latest distribution of TeX Live from [Tex Users Group](https://www.tug.org/texlive/). 
Then, download this repository and run the following command from your preferred shell, such as command prompt, in that folder's directory: $ xelatex resume.tex $

Alternatively, you can upload this template or access the base template for this resume and edit it with Overleaf, an online LaTeX editor. If you are running into compile errors, make sure you are using the XeTeX compiler available in the Overleaf settings.

* [**Edit Resume on OverLeaf.com**](https://www.overleaf.com/latex/templates/awesome-cv/tvmzpvdjfqxp)
* [**Edit Cover Letter on OverLeaf.com**](https://www.overleaf.com/latex/templates/awesome-cv-cover-letter/pfzzjspkthbk)

Preview:

![Resume Image](link)

## Quick Start Guide

You can jump into this template by editing the code in 'resume.tex'. 
Try changing the appearance of elements by commenting out style tags by adding '%' in the code within 'awesome-cv.cls'. 
For an example, you can left-justify your name in the resume header by finding the '\makecvheader' section and commenting `\begin{center}` and `\end{center}` 

You can easily change emphasis colours. Replace the color in the following entry near line 197 of 'awesome-cv.cls':
'''
\newcommand*{\sectionstyle}[1]{{\fontsize{16pt}{1em}\bodyfont\bfseries\color{blue}\@sectioncolor #1}} 
'''
Try the colors predefined by Font Awesome: `awesome`, `awesome-emerald`, `awesome-skyblue`, `awesome-red`, `awesome-pink`, `awesome-orange`, `awesome-nephritis`, `awesome-concrete`, `awesome-darknight`. Find more colors in the color config around line 100. Use your own additional colors by defining HTML color codes in `awesome-cv.cls` using `\definecolor`.

Add custom sections using `\cvsection`:

```
\cvsection{<Section Name>}
  \begin{cventries}
    \cventry
    {<Title>}
    {<Section Header>}
    {<Location>}
    {<Date>}
    {
      \begin{cvitems}
        \item{<bullet point 1>}
        \item{<bullet point 2>}
      \end{cvitems}
    }
  \end{cventries}
```

Credit to the original LaTeX Resume Template Source:
https://github.com/posquit0/Awesome-CV

```
