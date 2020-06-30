<div align="center">
 
  <a href="https://raw.githubusercontent.com/IliaZenkov/LaTeX-Resume/master/example/Resume.pdf">
    <img alt="Example Resume" src="https://img.shields.io/badge/resume-pdf-green.svg" />
   <a href="https://raw.githubusercontent.com/IliaZenkov/LaTeX-Resume/master/example/Cover%20Letter.pdf">
    <img alt="Example Coverletter" src="https://img.shields.io/badge/coverletter-pdf-green.svg" />
  </a>
</div>


This is my resume - a heavily modified fork of [awesome-cv](https://github.com/posquit0/Awesome-CV). Please use this template for your own job-hunting needs as you see fit!


## Setup

I recommend downloading the latest distribution of TeX Live from [Tex Users Group](https://www.tug.org/texlive/). 
Then, download this repository and run the following command from your preferred shell (e.g bash or cmd.exe if you use Windows) in that folder's directory: ``` $ xelatex resume.tex $ ```.


## Preview

| Resume | Cover Letter |
|:---:|:---:|
| ![Resume](https://raw.githubusercontent.com/IliaZenkov/LaTeX-Resume/master/example/resume.png)  | ![Cover Letter](https://raw.githubusercontent.com/IliaZenkov/LaTeX-Resume/master/example/cover%20letter.png)

## Quick Start Guide

You can jump into this template by editing the code in ```resume.tex.```
Try changing the appearance of elements by commenting out style tags with ```%``` in the code within ```awesome-cv.cls```. 
For an example, you can left-justify your name in the resume header by finding the ```\makecvheader``` section and commenting out ```\begin{center}``` and ```\end{center}```.

Add custom sections using the ```\cvsection``` command:

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


As another example, you can easily change emphasis colours. Replace the color in the following entry near line 197 of ```awesome-cv.cls```:
```
\newcommand*{\sectionstyle}[1]{{\fontsize{16pt}{1em}\bodyfont\bfseries\color{blue}\@sectioncolor #1}} 
```
Try the colors predefined by Font Awesome: `awesome`, `awesome-emerald`, `awesome-skyblue`, `awesome-red`, `awesome-pink`, `awesome-orange`, `awesome-nephritis`, `awesome-concrete`, and `awesome-darknight`. Find more colors in the color config around line 100. Use your own additional colors by defining HTML color codes in ```awesome-cv.cls``` using ```\definecolor```. 

Finally, do check out all the wonderful icons provided by [Font Awesome](https://fontawesome.com/) in ```fontawesome.sty``` in this repository.

## Super Quick Start Guide ;)

If you have trouble compiling this repository with LaTeX, you can start by accessing the base template for [awesome-cv](https://github.com/posquit0/Awesome-CV) and edit it with [Overleaf](Overleaf), an online LaTeX editor. If you are running into compile errors, make sure you are using the XeTeX compiler available in the Overleaf settings.

* [**Edit Resume on OverLeaf.com**](https://www.overleaf.com/latex/templates/awesome-cv/tvmzpvdjfqxp)
* [**Edit Cover Letter on OverLeaf.com**](https://www.overleaf.com/latex/templates/awesome-cv-cover-letter/pfzzjspkthbk)

Cheers and happy job hunting!
